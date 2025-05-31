<template>
  <div id="quiz-container">
    <h1>Quiz das Plantas Perdidas</h1>
    <h1 id="pergunta" :text="pergunta"> </h1>
    <h1 id="opcoes" :value="pergunta"> </h1>
    <button id="proximo">Próxima</button>
  </div>
</template>

<script>
  export default {
    name: "quiz",
    data() {
      return {
        pergunta: null,
        opcoes: []
      }
    },
    methods: {
      async get_perguntas() {
        const req = await fetch("http://localhost:3000/quiz")
        const data = await req.json();

        console.log(data);
        this.pergunta = data.pergunta;
        this.opcos = data.opcoes;
      }
    }
  }
</script>

<style scoped>
  body {
    background-size: cover;
    font-family: 'Georgia', serif;
    color: #4b3a1f;
    text-align: center;
    padding: 50px;
  }

  #quiz-container {
    background-color: rgba(255, 248, 220, 0.9);
    padding: 30px;
    border-radius: 15px;
    max-width: 600px;
    margin: auto;
    box-shadow: 0 0 20px rgba(0,0,0,0.3);
  }

  button {
    margin-top: 20px;
    padding: 10px 25px;
    background: #d6ad54;
    border: none;
    color: #fff;
    font-weight: bold;
    border-radius: 10px;
    cursor: pointer;
  }
</style>