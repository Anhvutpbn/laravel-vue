<template>
	<div>
		<h2>
			Day la homepage
		</h2>
	</div>
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