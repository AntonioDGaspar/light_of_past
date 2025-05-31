<template>
  <main>
    <h1> Estes são os Arquivos relacionados à Plantas que detemos em nosso Site: </h1>
    <section id="artigos">
      <section id="posts">
        <router-link to="/mandragora">
          <div class="flower">
            <div class="plantas" id="planta01">
              <img src="@/../public/img/mandragora01.jpg" alt="Imagem de Mandrágora" class="img_plantas" id="img_planta01">
              <h2> Mandrágora: Az Planta que Grita </h2>
              <p class="txt_plantas">
                Enraizada em lendas e gritos, esta planta já foi temida como um ser vivo entre os vivos. Você ousa conhecer sua história?
              </p>
            </div>
          </div>
        </router-link>
        <router-link to="/belladona">
          <div class="plantas" id="planta02">
            <img src="@/../public/img/belladona02.jpg" alt="Imagem de Belladona" class="img_plantas" id="img_planta02">
            <h2> Belladonna – A Flor dos Dois Mundos </h2>
            <p>
              Já foi o toque da beleza... e da morte. A Belladona seduz e envenena com a mesma elegância. Descubra seu duplo papel na história.
            </p>
          </div>
        </router-link>
        <router-link to="/datura">
          <div class="flower">
            <div class="plantas" id="planta03">
              <img src="@/../public/img/datura01.jpg" alt="Imagem de Datura" class="img_plantas" id="img_planta03">
              <h2> Datura – A Trombeta do Inferno </h2>
              <p class="txt_plantas">
                Usada por xamãs, bruxas e envenenadores — a Datura guarda segredos entre o êxtase e a loucura. Pronto para atravessar o véu?
              </p>
            </div>
          </div>
        </router-link>
      </section>
    </section>
  </main>
</template>

<script>
  export default {
    name: "plantas"
  }
</script>

<style scoped>
  main {
    text-align: center;
  }

  main > h1 {
    margin: 40px
  }

  section#artigos {
    background-color: burlywood;
    padding: 50px;
    width: 800px;
    margin: auto;
    border-radius: 10px;
    box-shadow: 3px 3px 7px #222222c7;
  }

  #posts {
    display: flex;
    text-align: center;
    align-items: center;
    justify-content: center;
    flex-direction: column;
  }

  div.flower {
    display: flex;
    position: relative;
  }

  .plantas {
    display: flex;
    justify-content: flex-end;
    width: 700px;
    height: 500px;
    background-color: #222;
    margin: 0px 50px 50px 50px;
    box-shadow: 1px 1px 13px 2px rgba(0, 0, 0, 0.678);
    cursor: pointer;
  }

  #planta01 {
    border-start-end-radius: 55%;
    border-end-start-radius: 55%;
  }

  div#planta01 > h2, div#planta03 > h2 {
    position: absolute;
    top: 220px;
    right: 90px;
    font-size: 1.12em;
  }

  div#planta02 > h2 {
    margin: 20px;
  }

  #planta02 {
    flex-direction: column;
    justify-content: center;
    align-items: center;
    border-radius: 50px;
  }

  #planta03 {
    border-start-end-radius: 55%;
    border-end-start-radius: 55%;
  }

  img.img_plantas {
    width: 270px;
    height: 270px;
    box-shadow: 6px 6px 13px 0px rgba(0, 0, 0, 0.678);
  }

  img#img_planta01, img#img_planta03 {
    border-radius: 50%;
    position: absolute;
    top: 20px;
    right: 420px;
  }

  img#img_planta02 {
    border-radius: 10px;
    margin: 20px;
  }

  .plantas > p {
    width: 300px;
    padding: 20px;
    color: bisque;
    font-size: 1.3em;
  }

  .txt_plantas {
    position: absolute;
    top: 260px;
    right: 85px;
  }

  .plantas:hover {
    background-color: rgb(185, 179, 171);
    width: 720px;
    height: 520px;
    transition: 1s;
  }

  @keyframes vento {
    0%, 100% { transform: rotate(0deb); }
    50% { transform: rotate(2deg); }
  }

  #planta01, #planta03 {
    animation: vento 3s ease-in-out infinite;
  }
</style>