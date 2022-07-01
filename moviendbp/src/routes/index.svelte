<script contextmenu="module">
	const apiKey = dda0d99160a176b43d0b9af81da127fc;

	export async function load({ fetch }) {
		const res = await fetch(
			`https://api.themoviedb.org/3/movie/popular?api_key=${apiKey}&language=en-US&page=1`
		);

        const data = await res.json();
	}
</script>
