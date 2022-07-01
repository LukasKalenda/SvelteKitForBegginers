<script context="module">
	

	export async function load({ fetch }) {
		const res = await fetch(
			`https://api.themoviedb.org/3/movie/popular?api_key=dda0d99160a176b43d0b9af81da127fc&language=en-US&page=1`
		);

		const data = await res.json();
        console.log(data);
		if (res.ok) {
			return {
				props: { popular: data.results }
			};
		}
	}
</script>

<script>
    import PopularMovies from "../components/PopularMovies.svelte";
    export let popular;
</script>

<section>
    <PopularMovies {popular}/>
</section>
