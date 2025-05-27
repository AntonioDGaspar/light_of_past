<template>
  <main>
    <div id="banner">
      <p> 
        Misteriosa e perigosa, a Belladona marcou presença em antigos rituais, curas e envenenamentos. Também chamada de “Bela Dona”, essa planta fascinou alquimistas e curandeiros por séculos. No Luz do Passado, exploramos sua origem, usos e o impacto que deixou na história.
      </p>
    </div>
    <section class="normal">
      <h2> Origem e Etimologia </h2>
      <p>
        A Atropa belladonna é nativa da Europa, Norte da África e partes da Ásia Ocidental. Seu nome vem da deusa grega Átropos, uma das três Moiras responsáveis por cortar o fio da vida humana. O nome belladonna (“mulher bonita”, em italiano) surgiu no Renascimento, quando a planta foi usada como cosmético.
      </p>
      <p>
        Belladonna é uma planta perene com folhas ovais largas e flores arroxeadas em forma de sino. Seus frutos — pequenas bagas negras brilhantes — são especialmente traiçoeiros: doces no sabor, mas mortais. Todas as partes da planta são venenosas, especialmente as raízes.
      </p>
    </section>
    <section class="imagem" id="img1">
      <h2> Usos Históricos e Medicinais </h2>
        <p>Desde a antiguidade, a Belladonna foi usada como:</p>
        <ul>
            <li>Analgésico e sedativo, citado por Hipócrates e Galeno.</li>
            <li>Cosmético: mulheres italianas aplicavam extratos nos olhos para dilatar as pupilas.</li>
            <li>Anestésico rudimentar em procedimentos cirúrgicos medievais.</li>
            <li>Ingrediente em poções e venenos, popular entre nobres e espiões renascentistas.</li>
        </ul>
        <p>Apesar disso, seu uso era arriscado — bastava uma pequena dose a mais para provocar alucinações, convulsões ou a morte.</p>
    </section>
    <section class="normal">
        <h2> Belladonna e o Ocultismo </h2>
        <p>
          Na Idade Média e no Renascimento, a planta era associada a práticas mágicas e bruxaria. Pomadas contendo Belladonna, aplicadas sobre a pele ou mucosas, produziam efeitos alucinógenos, levando algumas tradições a acreditarem que ela possibilitava "voos espirituais".
        </p>
        <p>
          Ela fazia parte dos unguentos das "bruxas voadoras" e estava ligada a rituais de comunicação com espíritos, proteção e até necromancia.
        </p>
    </section>
    <section class="imagem" id="img2">
        <h2> Declínio e Legado </h2>
        <p>
          Com o avanço da medicina científica, a Belladonna foi sendo substituída por medicamentos mais seguros. Ainda hoje, derivados como a atropina são usados em oftalmologia e anestesia — mas com controle rigoroso de dosagem.
        </p>
        <p>
          A Belladonna permanece como símbolo do perigo elegante, uma planta que encantou com sua beleza e matou com seu veneno.
        </p>
    </section>
    <section class="normal">
      <p> 
        A Belladonna nos mostra como a linha entre cura e destruição sempre foi tênue no passado. Seu legado permanece entrelaçado com histórias de beleza, morte e misticismo. Ao explorarmos sua trajetória, revivemos o conhecimento que nossos antepassados cultivaram com admiração e temor. No Luz do Passado, redescobrir a Belladonna é lembrar que, na natureza, até o mais belo pode esconder segredos sombrios — e que o esquecimento desses saberes pode nos afastar de quem fomos.
      </p>
    </section>
  </main>
</template>

<script>
    export default {
        name: "plantas-belladona"
    }
</script>

<style scoped>
  #banner {
    background-image: url("@/../public/img/belladona02.jpg");
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
    background-image: url(@/../public/img/belladona01.jpg);
    background-size: cover;
  }

  section#img2 {
    background-image: url(@/../public/img/belladona03.jpg);
  }
</style>