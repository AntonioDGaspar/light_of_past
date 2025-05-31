<template>
  <div class="home">
    <banner />
    <section id="apresentacao">
       <div class="div_apresentacao" id="div_ap01">
        <img src="@/../public/img/old_library.jpg" alt="Descrição do Texto" class="img_apresentacao" id="img_ap01">
        <p class="txt_apresentacao" id="txt_ap01">
          Este é um santuário digital para mentes curiosas e corações inquietos que acreditam que o progresso não é só o que está por vir, mas também o que ficou para trás.
        </p>
      </div>
      <div class="div_apresentacao" id="div_ap02">
        <img src="@/../public/img/old_watch01.jpg" alt="Descrição do Texto" class="img_apresentacao" id="img_ap02">
        <p class="txt_apresentacao"> 
          O "Luz do Passado" nasce da necessidade de reacender memórias tecnológicas, invenções pioneiras e ideias ousadas que, por algum motivo, foram deixadas nas sombras.      
       </p>
      </div>
      <div class="div_apresentacao" id="div_ap03">
        <p class="txt_apresentacao" id="txt_ap03">
          Nem toda grande invenção sobreviveu ao tempo. Algumas foram esquecidas, soterradas pelo silêncio da história. Neste espaço, resgatamos ideias geniais que desapareceram antes de brilhar. Em cada engrenagem esquecida, há uma história que clama para ser ouvida.
        </p>
        <img src="@/../public/img/engrenagem.png" alt="Descrição do Texto" class="img_apresentacao" id="img_ap03">
      </div>
    </section>
    <h1 id="titulo_posts"> Postagens em Destaque </h1>
    <section id="postagens">
      <router-link to="/mandragora">
        <div class="div_postagens">
          <img src="@/../public/img/mandragora01.jpg" alt="Descrição do Texto" class="img_postagens" id="img_post1">
          <p> Mandrágora </p>
        </div>
      </router-link>
      <router-link to="/belladona">
        <div class="div_postagens">
          <img src="@/../public/img/belladona02.jpg" alt="Descrição do Texto" class="img_postagens" id="img_post2">
          <p> Belladona </p>
        </div>
      </router-link>
      <router-link to="/datura">
        <div class="div_postagens">
          <img src="@/../public/img/datura01.jpg" alt="Descrição do Texto" class="img_postagens" id="img_post3">
          <p> Datura </p>
        </div>
      </router-link>
    </section>
  </div>
</template>

<script>
  import banner from "../components/banner.vue"

  export default {
     name: 'HomeView',
     components: {
      banner
     }
  }
</script>

<style scoped>
  #apresentacao {
    width: 90%;
    margin: auto;
    margin-top: -40px;
    text-align: center;  }

  .div_apresentacao {
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    margin-bottom: 50px;
    height: 450px;
    width: 100%;
  }

  #div_ap01 {
    justify-content: flex-end;
    background-color: blanchedalmond;
    border-top-right-radius: 50px;
    border-top-left-radius: 50px;
  }

  #div_ap02 {
    height: 500px;
    background-color: beige;
    flex-direction: column;
  }
  
  #div_ap03 {
    justify-content: flex-start;
    background-color: bisque;
  }

  .txt_apresentacao {
    color: var(--cor01);
    width: 600px;
    height: 200px;
    margin: 15px 50px 50px 0px;
    font-size: 1.5em;
    text-align: justify;
    line-height: 1.5;
  }

  #txt_ap01 {
    margin-top: 100px;
  }

  #txt_ap03 {
    margin-left: 100px;
  }

  .img_apresentacao {
    width: 150px;
    height: 200px;
    margin: 50px;
  }

  #img_ap01 {
    width: 300px;
    height: 300px;
    border-radius: 50px;
    box-shadow: 0px 1px 10px #222;
  }

  #img_ap02 {
    width: 300px;
    height: 450px;
    border-radius: 50%;
    box-shadow: 0px 5px 10px #222;
  }

  #img_ap03 {
    width: 500px;
    height: 500px;
    border-radius: 50px;
    animation: girar 20s linear infinite;
  }

  #titulo_posts {
    text-align: center;
    margin: 20px;
  }

  #postagens {
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
  }

  .div_postagens {
    display: inline-block;
    height: 350px;
    width: 400px;
    margin: 20px;
    background-color: var(--cor01);
    border-top-left-radius: 50px;
    border-bottom-right-radius: 50px;
    cursor: pointer;
  }

  .img_postagens {
    margin: 20px;
    width: 300px;
    height: 200px;
    border-radius: 10px;
  }

  .div_postagens > p {
    font-size: 2em;
    color: bisque;
  }

  .div_postagens:hover {
    width: 420px;
    height: 370px;
    background-color: burlywood;
    transition: 0.5s;
  }

  @keyframes girar {
    from { transform: rotate(0deg); }
    to { transform: rotate(360deg); }
  }
</style>