<script>
    import marked from "marked"
    $: markedtext = `# Mon titre
* apple
* orange
* banana`
</script>
<h2>Exo 2</h2>
<div class="container">
    <div class="col text-marked">
        <h2>Markdown</h2>
        <textarea bind:value={markedtext} cols="30" rows="10"></textarea>
    </div>
    <div class="col text-result">
        <h2>Results</h2>
        <p class="result">{@html marked(markedtext)}</p>
    </div>
</div>

<style>
    .container {
        display: flex;
        flex-direction: row;
        gap: 10px;
    }
    .col {
        width: 500px;
        border: 2px solid springgreen;
    }
</style>