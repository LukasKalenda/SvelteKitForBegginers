<script>

    let count = 0;

    function pricitani(){
        count +=1;
    }
</script>


<h1>Number: {count}</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
    
    <button>Já jsem tlacitko</button>
    <p>Zde si klikni na about page <a href="/about">About</a></p>

    <button on:click={pricitani}>Pricitani</button>






    <style>
        p{
            font-size: 2rem;
        }
    </style>