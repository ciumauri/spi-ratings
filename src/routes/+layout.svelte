<script lang="ts">
	import Cabecalho from '$lib/componentes/layout/Cabecalho.svelte';
	import Rodape from '$lib/componentes/layout/Rodape.svelte';
	import '../app.css';
</script>

<div class="container-principal">
	<Cabecalho />
	<slot><!-- optional fallback --></slot>
	<Rodape />
</div>

<style>
	.container-principal {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	/* .estilo-principal {
		text-align: center;
		padding: 0 5vw 3.375rem;
		flex: 1;
	}

	.minha-lista-container {
		margin-bottom: 2rem;
	}

	.divisoria {
		width: 40vw;
		height: 2px;
		background-color: var(--verde);
		margin: 0 auto;
	} */
</style>
