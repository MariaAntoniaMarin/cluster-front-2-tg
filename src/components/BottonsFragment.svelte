<script>
	//import Info from './Info.svelte';

    function infoClick() {
		document.location.href='Info/';
	}
</script>

<div class="box">
    <button class="button is-primary is-outlined is-medium" on:click={infoClick}>
        Acerca de Algoritmos
    </button>
    <button class="button is-info is-outlined is-medium">Realiza Agrupamiento K-Means</button>
    <button class="button is-link is-outlined is-medium">Numero optimo de grupos</button>
</div>

<style>
    .box {
        width: 500px;
        
        display: flex;
        flex-direction: column;
        gap: 1em;
    }
</style>
