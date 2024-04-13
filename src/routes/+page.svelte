<script>
    let text = "8=D"
    const crescer = () => {
        text = text.slice(0, text.length-1) + "=D"
    }
</script>

<svelte:head>
    <title> Yejiverso </title>
</svelte:head>
<h1>Pinto</h1>
<p>{text}</p>
<button on:click={crescer}> Fazer o pinto crescer </button>