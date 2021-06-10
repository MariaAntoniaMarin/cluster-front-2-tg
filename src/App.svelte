<script>
	import { Router, Route, Link } from "svelte-routing";
	import Index from "./pages/Index.svelte";
	import Home from "./pages/Home.svelte";
	import About from "./pages/About.svelte";
	export let url = ""; //This property is necessary declare to avoid ignore the Router
</script>

<Router url="{url}">
	<nav>
	   <Link to="/">Home</Link>
	   <Link to="index">Index</Link>
	   <Link to="about">About</Link>
	 </nav>
	 <div>
	   <Route path="about" component="{About}" />
	   <Route path="index" component="{Index}" />
	   <!--for now the router just support case sensitive,
		   one workaround colud be add two time the route
		   Example.
		  <Route path="About" component="{About}" /> 
	   -->
	   <Route path="/"><Home /></Route>
	 </div>
</Router>
   