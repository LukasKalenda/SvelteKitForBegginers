<script>
export let popular;
console.log(popular);
</script>

<h1>Popular Movies</h1>
<div class="popular-movies">
	<div class="movie"/>

    {#each popular as movie}
    <h1>{movie.title}</h1>
    {/each}

</div>
