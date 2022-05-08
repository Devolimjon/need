<script lang="ts">
	import { Router, Link, Route } from "svelte-navigator";
</script>
<main class="container">
  <img class="i-am" src="https://yt3.ggpht.com/Vqx6B1cyJn0gKen7ngl3k763hiZMfQWWpxGdseuFvdWaMXwfUi68fi2Kf8YCkNqQkwXCcsDRuw=s108-c-k-c0x00ffffff-no-rj" alt="">
  <h1>Makhmudov Olimjon</h1>
  <br>
  <h3>IT IS MY PORTFOLIO</h3>
  <div class="go">
    <Router>
          <Link class="btn btn-primary" style="text-decoration: none;font-weight: 700; color: white;" to="/myself">myself  <i class="fa-solid fa-right-long"></i></Link>
          <br>
          <Link class="btn btn-primary" style="text-decoration: none;font-weight: 700; color: white;" to="/register">my projects  <i class="fa-solid fa-right-long"></i></Link>
        <Route path="/myself">
        </Route>
    </Router>
  </div>
</main>
<style>
  main{
    height: 65vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
  .i-am{
    border-radius: 50%;
    width: 160px;
  }
  .go{
    padding-top: 30px;
    display: flex;
    flex-direction: column;
    gap:3px;
  }
  .btn{
    color: white;
  }
</style>