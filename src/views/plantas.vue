<template>
  <main>
      <p> Estes são os Arquivos relacionados à Plantas que detemos em nosso Site: </p>
      <section id="posts">
        <div class="plantas" id="planta01">
          <img src="" alt="">
          <p>
            Enraizada em lendas e gritos, esta planta já foi temida como um ser vivo entre os vivos. Você ousa conhecer sua história?
          </p>
        </div>
        <div class="plantas" id="planta02">
          <p>
            Já foi o toque da beleza... e da morte. A Belladona seduz e envenena com a mesma elegância. Descubra seu duplo papel na história.
          </p>
        </div>
        <div class="plantas" id="planta03">
          <p>
            Usada por xamãs, bruxas e envenenadores — a Datura guarda segredos entre o êxtase e a loucura. Pronto para atravessar o véu?
          </p>
        </div>
      </section>
  </main>
</template>

<script>
  export default {
    name: "plantas",
    components: {
      navBar
    }
  }
</script>

<style scoped>
  main {
    text-align: center;
  }

  main > p {
    margin: 20px;
    
  }

  #posts {
    display: flex;
    text-align: center;
    align-items: center;
    justify-content: center;
    flex-direction: column;
  }

  #banner {
    background-image: url("@/../public/img/manha.jpg");
    background-size: cover;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100vw;
    height: 500px;
    box-shadow: 0px 3px 10px rgba(0, 0, 0, 0.705);
    margin-bottom: 50px;
  }

  #banner p {
    font-size: 3em;
    color: var(--cor_Principal);
    width: 500px;
    margin-left:30px;
    padding: 5px 5px 5px 10px;
    background-color: #222222da;
    border-radius: 10px;
    font-size: 2.7em;
  }

  .plantas {
    width: 700px;
    height: 500px;
    background-color: blue;
    margin: 50px;
    border-radius: 10px;
  }

  #planta01 {

  }

  #planta02 {
    justify-self: flex-end;
  }

  #planta03 {

  }
</style>