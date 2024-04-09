<style>
    body {
        font-family: "Lucida Console", "Courier New", monospace;
        text-align: center;
    }
</style>

<script>

    let userinput = '';
    function handleChange(event) {
        userinput = event.target.value;
    }
    function gotoPage(event) {
        window.location.href = `https://www.google.com/search?q=${userinput}`;
    }
</script>

<body>
    <h2>Google Searcher (I Don't Know Why I Made This)</h2>
    <input type="text" bind:value={userinput} on:input={handleChange}>
    <button on:click={gotoPage}>Search</button>
</body>
