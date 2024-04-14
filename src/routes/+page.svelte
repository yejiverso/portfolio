<script>
    let text = "🎔"
    const grow = () => {
        text += "🎔"
    }
</script>

<svelte:head>
    <title> Portfolio </title>
</svelte:head>
<div class="audiow">

    <audio controls autoplay>
        <source src="wave to earth - seasons.mp3" type="audio/mpeg">
      Your browser does not support the audio element.
    </audio>
</div>
    <div class="jmk">
        <p>
            Júlia Kraus, saiba que enquanto eu existir, você vai ter eternamente alguém do seu lado. Quero ser sua parceirinha de tudo, no amor, na amizade, nos momentos bons e mais ainda nos ruins. Você é a pessoa que eu quero ir quando meu peito apertar e o mundo parecer cruel demais, sua voz tem o poder de curar tudo pra mim, queria ser a sua musa pra ser eternamente adorada pelos lindos olhos que você tem. Não consigo invejar bilionários, famosos, que seja, eu sou amada pela Júlia. Quão mais sortuda eu poderia ser? a boquinha linda dela agora é minha, eu vou ser a pessoa que vai amar ela do bom dia até o boa noite, euzinha, mais ninguém. Acho que o paraíso realmente existe, me dou conta disso toda vez que olho pra você. Eu te amo, meu amor. Como é bom te amar, juju. Obrigada por esse privilégio.        </p>
        <p class="hearts">{text}</p>
        <button on:click={grow}>Aperte aqui</button>
        </div>
<style lang="scss">
    @font-face {
        font-family: sedan;
        src: url("/Sedan-Regular.ttf")
    }
   .jmk{
        font-family: sedan;
        font-size: large;
        padding: 1vh 1vw;
        margin: 17vh auto;
        height: 45vh; 
        width: 65vh;
        border-style: solid;
        box-shadow: 5px 5px #ff748c, 10px 10px #ff8da1, 15px 15px #ffa7b6, 20px 20px #ffdae0;
    }
    .hearts {
        margin-top: 8vh;
    }
    button {
        border-style: none;
        background-color: #ff748c;
        padding: 15px;
        border-radius: 15px;
    }
    .audiow {
        margin: 0 auto;
        width: 90vw;
        display: flex;
        justify-content: center;
    }
</style>