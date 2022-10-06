<script>
  // pages
  import Login from "./pages/Login.svelte";
  import MeetUs from "./pages/MeetUs.svelte";
  import Home from "./pages/Home.svelte";
  import About from "./pages/About.svelte";
  // router
  import { Router, Route, Link } from "svelte-routing";
</script>

<Router>
  <nav class="navbar">
    <Link to="/">Home</Link>
    <Link to="/about">About</Link>
    <Link to="/meetUs">MeetUs</Link>
    <Link to="/login">Login</Link>
  </nav>
  <Route path="/" component={Home} />
  <Route path="/about" component={About} />
  <Route path="/login" component={Login} />
  <Route path="/meetUs" component={MeetUs} />
</Router>
