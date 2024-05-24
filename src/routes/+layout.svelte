<script>
  import SideBar from "./SideBar.svelte";
  import "bootstrap/dist/css/bootstrap.min.css";
  import "./styles.css";
</script>

<svelte:head>
  <title>ArteCuliacan</title>
  <meta name="description" content="Svelte demo app" />
</svelte:head>

<body class="container-fluid">
  <main class="d-flex flex-nowrap">
    <div class="b-example-divider b-example-vr"></div>
	<SideBar/>
	  <slot/>
  </main>
</body>

<style>
  
  
</style>
