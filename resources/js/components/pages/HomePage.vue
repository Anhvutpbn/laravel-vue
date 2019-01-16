<template>
	<main class="container" role="main">
	    <div class="jumbotron">
	        <h1>
	            Navbar example
	        </h1>
	        <p class="lead">
	            This example is a quick exercise to illustrate how the top-aligned navbar works. As you scroll, this navbar remains in its original position and moves with the rest of the page.
	        </p>
	        <a class="btn btn-lg btn-primary" href="../../components/navbar/" role="button">
	            View navbar docs »
	        </a>
	    </div>
	</main>
</template>
<script type="text/javascript">
	export default {
		props: ['component'],
		mounted() {
			this.$emit('changeTitle', 'ta da doi duoc title')
			console.log(this.component)
		}
	}
</script>