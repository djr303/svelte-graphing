<script>
  import { Router, Link, Route } from "svelte-routing";
  import Home from "./pages/home/index.svelte";
  import SimplePath01 from "./pages/simplePath01/index.svelte";
  import SimplePath02 from "./pages/simplePath02/index.svelte";
 
  export let url = "";
</script> 
 
<Router url="{url}">
  <nav>
    <Link to="/">Home</Link> |&nbsp;
    <Link to="simple-path-01">Simple path 01</Link> |&nbsp; 
    <Link to="simple-path-02">Simple path 02</Link>
  </nav>
  <div>
    <Route path="/" component="{Home}" />
    <Route path="simple-path-01" component="{SimplePath01}" />
    <Route path="simple-path-02" component="{SimplePath02}" />
  </div>
</Router>