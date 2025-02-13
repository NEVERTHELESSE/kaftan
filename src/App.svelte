<script>
  import { Router, Route, Link } from "svelte-routing";
  import Home from "./pages/home/Home.svelte";
  import About from "./pages/about/About.svelte";
</script>

<Router>
  <nav>
    <Link to="/">Home</Link>
    <Link to="/about">About</Link>
  </nav>

  <Route path="/" component={Home} />
  <Route path="/kaftan" component={Home} />
  <Route path="/about" component={About} />
</Router>
