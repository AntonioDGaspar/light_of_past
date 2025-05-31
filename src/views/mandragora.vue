<template>
  <div>
    <div id="banner">
      <p> 
        Por séculos, Mandrágora habitou o imaginário popular como uma planta capaz de curar doenças, induzir estados alterados de consciência e até soltar gritos mortais ao ser arrancada do solo. Neste artigo, exploramos as origens, os usos históricos e os mitos que cercam essa planta envolta em mistério e superstição.
      </p>
    </div>
    <section class="normal">
      <h2> Mandrágora: A Planta que Grita </h2>
      <p>
        A mandrágora (do gênero Mandragora) é uma planta nativa do Mediterrâneo e do Oriente Médio, profundamente enraizada nas tradições do Antigo Egito, Grécia e Europa Medieval. Sua raiz, muitas vezes com forma humanoide, foi associada a rituais mágicos, feitiçaria e medicina arcaica.
      </p>
      <p>
        Na Grécia antiga, era usada como afrodisíaco e anestésico. Os romanos acreditavam que ela podia curar tudo, desde dor de dente até esterilidade. Na Idade Média, era um ingrediente essencial nas poções de bruxas e alquimistas.
      </p>
    </section>
    <section class="imagem" id="img1">
      <h2> Lendas e Mitos </h2>
      <p>
        A lenda mais conhecida da mandrágora diz que, ao ser arrancada do solo, ela solta um grito tão alto que mata quem o ouve. Para evitar isso, os antigos ensinavam que se deveria amarrar um cão à raiz e forçá-lo a correr — assim, o cão morreria no lugar do humano.
      </p>
      <p>
        Essa crença popularizou a planta nos grimórios (livros de magia) e nos contos medievais. A ideia do “grito” pode ter vindo da forte reação narcótica da planta, que causa alucinações, inconsciência e até morte se mal utilizada.
      </p>
    </section>
    <section class="normal">
      <h2> Usos Medicinais e Místicos </h2>
      <ul>
        <li> Anestésico: triturada e colocada sob o nariz antes de cirurgias rudimentares. </li>
        <li> Sonífero potente: usada para induzir sono profundo, quase coma. </li>
        <li> Afrodisíaco: em poções de amor e fertilidade. </li>
        <li> Proteção espiritual: era colocada sob camas ou enterrada perto da porta como talismã contra espíritos malignos. </li>
      </ul>
    </section>
  </div>
</template>

<script>
    export default {
        name: "plantas-mandragora"
    }
</script>

<style scoped>
    #banner {
      background-image: url("@/../public/img/mandragora01.jpg");
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
      padding: 15px;
      background-color: rgba(222, 184, 135, 0.904);
      border-radius: 10px;
    }

    section {
      padding: 40px;
      line-height: 2em;
      font-family: var(--fonte2);
      font-size: 1.5em;
      width: 800px;
      margin: auto;
      border-radius: 30px;
      margin-bottom: 40px;
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

    section.imagem > p {
      width: 800px;
      background-color: rgba(0, 0, 0, 0.644);
      text-shadow: 1px 1px 0px black;
      padding: 10px;
    }

    section#img1 {
      background-image: url(@/../public/img/mandragora02.jpg);
      background-size: cover;
    }

    section#img2 {
      background-image: url(@/../public/img/Fundo.jpg);
    }
</style>