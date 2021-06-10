
<script>
	import HeaderChart from './HeaderChart.svelte';
  import BottonsFragment from './BottonsFragment.svelte';
</script>


<div class='header-chart'>
    <HeaderChart />
</div>

<div class='title'>
    <h1>Agrupamiento de datos GPS con algoritmo Kmeans</h1>
</div>

<div class='bottons'>
    <BottonsFragment/>
</div>

<div class='text'>
    <p>Aplicación web para el agrupamiento validado de datos de georreferenciación usando el algoritmo k-means.</p><br>
    <p>Trabajo de grado de la Universidad nacional sede manizales.</p>
</div>

<style>

div.header-chart {
  height: 300px;
  width: auto;
}

div.title {
  text-align: center;
}

div.text {
  font-size: large;
  position: absolute;
  top: 390px;
  right: 100px;
  width: 500px;
  padding: 20px;
}

</style>
