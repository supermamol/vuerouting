<template>
	<div id="app">
		<router-link class="link" :to="{ path: '/hello', query: { name: 'Foo' }}">Say hello</router-link>
		<router-link class="link" :to="{ path: '/goodbye', query: { name: 'Foo' }}">Say goodbye</router-link>
		<br>
		<router-view></router-view>
	</div>
</template>

<script>
	export default {
    name: 'app'
  }
</script>

<style>
	#app {
		margin: 60px;
	}

	.link {
		display: inline-block;
		padding: 10px;
	}

	.router-link-active {
		color: green;
	}
</style>