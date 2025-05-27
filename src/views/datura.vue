<template>
  <main>
    <div id="banner">
      <p> 
        Temida por muitos e reverenciada por outros, a Datura é uma flor que exala mistério. Com suas pétalas torcidas como trombetas, ela foi usada por feiticeiros, xamãs e curandeiros em rituais que buscavam cruzar os véus da realidade. Neste artigo, vamos explorar os usos, histórias e advertências deixadas por essa planta que ecoa como um chamado antigo, vindo das profundezas da alma humana.
      </p>
    </div>
    <section class="normal">
      <h2> Origem e Nomes Populares </h2>
      <p>
        A planta pode atingir até dois metros de altura, com folhas grandes e flores brancas ou roxas em forma de trombeta. Seus frutos são cápsulas espinhosas que se abrem ao secar, liberando dezenas de sementes. Todas as partes da Datura são extremamente venenosas.
      </p>
    </section>
    <section class="imagem" id="img1">
      <h2> Usos Rituais e Espirituais </h2>
        <p> 
            Na América pré-colombiana, culturas como os astecas e os xamãs andinos utilizavam a Datura em rituais religiosos e espirituais. Era considerada uma ponte entre o mundo dos vivos e o dos espíritos. Em alguns ritos, ela era usada para:
        </p>
        <ul>
            <li> Induzir visões e experiências extracorporais; </li>
            <li> Favorecer sonhos proféticos; </li>
            <li> Preparar guerreiros para batalhas, dando coragem (e inconsciência da dor); </li>
            <li> Iniciar jovens em rituais de transição e revelação. </li>
        </ul>
        <p>Apesar disso, seu uso era arriscado — bastava uma pequena dose a mais para provocar alucinações, convulsões ou a morte.</p>
    </section>
    <section class="normal">
        <h2> Perigos e Advertências </h2>
        <p> 
            Assim como a Belladonna, a Datura é uma planta de extremos. Seu consumo, mesmo em pequenas doses, pode provocar:
        </p>
        <ul>
            <li> Delírios prolongados; </li>
            <li> Amnésia; </li>
            <li> Comportamentos agressivos ou incoerentes; </li>
            <li> E, em muitos casos, a morte. </li>
        </ul>
        <p>
            Por isso, muitas culturas a tratavam com reverência e medo, jamais sendo manipulada sem preparação espiritual e conhecimento profundo.
        </p>
    </section>
    <section class="imagem" id="img2">
        <h2> A Datura na Europa e no Folclore </h2>
        <p>
          Levadas pelos colonizadores, espécies de Datura foram rapidamente associadas à bruxaria e ao ocultismo na Europa. Na Idade Média, ela foi apontada como ingrediente em poções de metamorfose e unguentos das bruxas.
        </p>
        <p>
          Textos antigos relatam que a Datura, quando queimada, liberava vapores usados para entrar em transe — algo que alimentou lendas sobre possessão, loucura e contatos com seres de outros planos.
        </p>
    </section>
    <section class="normal">
      <h2> Declínio e Curiosidade Moderna </h2>
      <p> 
        Hoje, a Datura é evitada por seu risco e seu estigma. Ainda assim, continua crescendo em locais abandonados, jardins sem supervisão e terrenos baldios. O que antes era vista como planta de poder, agora é considerada "mato perigoso" — um reflexo do quanto esquecemos de nosso passado místico.
      </p>
      <hr>
      <br>
      <h2> Conclusões </h2>
      <p>
        A Datura é uma das plantas mais enigmáticas da história humana. Seu uso nos leva a um tempo em que o conhecimento era passado por ritos, visões e experiências com o mundo invisível. No Luz do Passado, seu legado nos lembra de que os maiores mistérios não foram apagados — apenas enterrados sob o medo e o esquecimento. Conhecer a Datura é ouvir o sussurro de uma sabedoria antiga que pede cuidado, respeito e humildade.
      </p>
    </section>
  </main>
</template>

<script>
    export default {
        name: "plantas-datura"
    }
</script>

<style scoped>
  #banner {
    background-image: url("@/../public/img/datura01.jpg");
    background-size: cover;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100vw;
    height: 670px;
    box-shadow: 0px 3px 10px rgba(0, 0, 0, 0.705);
    margin-bottom: 50px;
  }

  #banner p {
    font-size: 2.3em;
    color: var(--cor_Secundaria);
    width: 900px;
    margin-left:30px;
    padding: 5px 5px 5px 10px;
    background-color: rgba(222, 184, 135, 0.801);
    border-radius: 10px;
  }

  section {
    padding: 10px;
    line-height: 2em;
    font-family: var(--fonte2);
    font-size: 1.5em;
    width: 800px;
    margin: auto;
    margin-bottom: 20px;
    border-top-left-radius: 30px;
    border-bottom-right-radius: 30px;
  }

  section p {
    text-align: justify;
    margin: 20px;
  }

  section.normal {
    background-color: lightgrey;
  }

  section.normal li {
    background-color: lightgrey;
  }

  section.imagem {
    background-color: burlywood;
    color: white;
    box-shadow: inset 6px 6px 13px 0px rgba(0, 0, 0, 0.678);
    background-size: cover;
    background-position: right center;
    background-attachment: fixed;
  }

  section.imagem > p, li {
    width: 700px;
    margin: auto;
    background-color: rgba(0, 0, 0, 0.644);
    text-shadow: 1px 1px 0px black;
    padding: 10px;
  }

  section.imagem li {
    list-style-position: inside;
  }

  section#img1 {
    background-image: url(@/../public/img/datura02.jpg);
    background-size: cover;
  }

  section#img2 {
    background-image: url(@/../public/img/datura03.jpg);
  }
</style>
