<template>
	<div id="app">
		<Header></Header>
		<Banner></Banner>
		<Projects></Projects>
	</div>
</template>

<script>
import Header from './components/layout/Header'
import Banner from './components/Banner'
import Projects from './components/Projects.vue'

export default {
	name: 'App',
	components: { Header, Banner, Projects }
}
</script>

<style>
*{
	margin: 0;
	padding: 0;
	box-sizing: border-box;
	font-size: 10px;
}
#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	color: #2c3e50;
}
</style>
