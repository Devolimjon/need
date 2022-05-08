<script lang="ts">
	import { Router, Link, Route } from "svelte-navigator";
	import Home from "./components/home.svelte";
	import Myself from "./components/myself.svelte";
</script>

<main>
	<Router>
		<header>
			<div>
				<img width="200px" src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/7a/Myself-Logo.svg/1694px-Myself-Logo.svg.png" alt="">
			</div>
			<div class="nav">
				<Link style="text-decoration: none;font-weight: 700;font-size:20pt;" to="/">HOME</Link>
				<Link style="text-decoration: none;font-weight: 700;font-size:20pt;" to="/myself">MYSELF</Link>
				<Link style="text-decoration: none;font-weight: 700;font-size:20pt;margin-right:10px" to="/register">MY-PROJECT</Link>
			</div>
		</header>
		  <Route path="/">
			<Home/>
		  </Route>
		  <Route path="/myself">
			<Myself/>
		  </Route>
	</Router>
</main>

<style>
	header{
		padding: 3px;
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		align-items: center;
		-webkit-box-shadow: 0px 49px 25px -2px rgba(34, 60, 80, 0.2);
        -moz-box-shadow: 0px 49px 25px -2px rgba(34, 60, 80, 0.2);
         box-shadow: 0px 49px 25px -2px rgba(34, 60, 80, 0.2);
		}
	.nav{
		display: flex;
		flex-direction: row;
		gap:50px
	}
</style>