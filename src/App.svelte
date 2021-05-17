<script>
window.document.body.classList.toggle('dark')
import { fade } from 'svelte/transition';

</script>

<main>
	
<h1 transition:fade>Crypto</h1>

<input type="text" placeholder="Password" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}"><br><br>
<button>Login</button>
</main>


<style>
	main {
		text-align: center;
		padding: 12em;
		max-width: 240px;
		margin: 0 auto;
		
	}
	
	:global(body.dark) {
		background-color: #1d3040;
	}

	button {
		background-color: #f76027;
		color: white;
		border: none;
		border-radius: 50px;
		padding: 0.75rem;
		text-transform: uppercase;
		
	}
	h1 {
		color: #ffffff;
		text-transform: uppercase;
		font-size: 7em;
		font-weight: 500;
		background-color: #1d3040;
	
	}
	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
	
</style>