<script>
	import '../app.css' // panda reset
	import { css } from 'styled-system/css';
</script>
<nav>
	<div class="container">
		<a href="/">Home</a>
		<a href="/dashboard">Dashboard</a>
		<a href="/settings">Settings</a>
	</div>
</nav>

<div class="container"> 
	<slot></slot>
</div>

<style>
	body {
		margin: 0;
	}

	nav {
		background-color: lightcyan;
		padding: 1rem 0rem;
	}

	a {
		color: blue;

		&:hover {
			text-decoration: underline;
		}
	}

	.container {
		max-width: 960px;
		margin: 0 auto;
	}
</style>

