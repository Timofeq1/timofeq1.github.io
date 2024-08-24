<script>
  import { Router, Link, Route } from "svelte-routing";
  import Home from "./routes/Home.svelte";
  import About from "./routes/About.svelte";
  import NotFound from './routes/NotFound.svelte';
</script>



<Router>
    <nav>
        <Link to="/">Home</Link>
        <Link to="/about">About</Link>
    </nav>

  <Route path="/" component={Home} />
  <Route path="/about" component={About} />
  <Route path="*" component={NotFound} />
</Router>

<style>
  nav {
    background-color: #333;
    padding: 1rem;
  }
  a {
    color: white;
    text-decoration: none;
    margin-right: 1rem;
  }
</style>
