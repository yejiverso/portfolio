<script>
    let text = "🎔"
    const grow = () => {
        text += "🎔"
    }
</script>

<svelte:head>
    <title> Portfolio </title>
</svelte:head>
    <div class="jmk">
        <p>
            Yeji nasceu em 26 de maio de 2000, em Jeonju-do. Em 2014, tornou-se membro do grupo de dança de Jeonju "Blue Rump (Jeonju Youth Dance Club)". Ela se tornou uma aluna na escola de dança Near Art Story no primeiro ano do ensino médio.
            Em dezembro de 2015, ela fez um teste para a JYP Entertainment com a música "Like Ooh-Ahh" do girl group TWICE.
            Apareceu pela primeira vez em agosto de 2016 no "JYP showcase". Em 2017, juntamente com as futuras integrantes de seu atual grupo (exceto Lia), apareceu no reality show da Mnet, Stray Kids, como parte da equipe feminina de pré-debut da JYP Entertainment. No final de 2018, ela se tornou participante do programa de sobrevivência "The Fan" da SBS, mas desistiu sem marcar pontos suficientes.
        </p>

        <audio autoplay>
            <source src="wave to earth - seasons.mp3" type="audio/mpeg">
          Your browser does not support the audio element.
        </audio>
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
        margin: 25vh auto;
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
</style>