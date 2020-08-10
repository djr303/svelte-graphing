<script>
  import { Router, Link, Route } from "svelte-routing";
  import Home from "./pages/home/index.svelte";
  import SimplePath01 from "./pages/simplePath01/index.svelte";
  import SimplePath02 from "./pages/simplePath02/index.svelte";
  import SimplePath03 from "./pages/simplePath03/index.svelte";
  import SimplePath04 from "./pages/simplePath04/index.svelte";
  import SimplePath05 from "./pages/simplePath05/index.svelte";
 
  export let url = "";
</script> 
 
<Router url="{url}">
  <nav>
    <Link to="/">Home</Link> |&nbsp;
    <Link to="simple-path-01">Simple path 01</Link> |&nbsp; 
    <Link to="simple-path-02">Simple path 02</Link> |&nbsp;
    <Link to="simple-path-03">Simple path 03</Link> |&nbsp;
    <Link to="simple-path-04">Simple path 04</Link> |&nbsp;
    <Link to="simple-path-05">Simple path 05</Link>
  </nav>
  <div>
    <Route path="/" component="{Home}" />
    <Route path="simple-path-01" component="{SimplePath01}" />
    <Route path="simple-path-02" component="{SimplePath02}" />
    <Route path="simple-path-03" component="{SimplePath03}" />
    <Route path="simple-path-04" component="{SimplePath04}" />
    <Route path="simple-path-05" component="{SimplePath05}" />
  </div>
</Router>