<template>
	<div id="app">
		<Header></Header>
		<Banner></Banner>
		<About></About>
		<Projects></Projects>
		<Courses></Courses>
		<Freelances></Freelances>
		<Contact></Contact>
		<Footer></Footer>
	</div>
</template>

<script>
import Header from './components/layout/Header'
import Banner from './components/Banner'
import About from './components/About'
import Projects from './components/Projects.vue'
import Courses from './components/Courses.vue'
import Freelances from './components/Freelances.vue'
import Contact from './components/Contact.vue'
import Footer from './components/layout/Footer.vue'

export default {
	name: 'App',
	components: { Header, Banner, Projects, About, Contact, Footer, Courses, Freelances }
}
</script>

<style>
*{
	margin: 0;
	padding: 0;
	box-sizing: border-box;
	font-size: 10px;
}
#app, * {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	color: #2c3e50;
	scroll-behavior: smooth;
}
a{
	text-decoration: none;
}
</style>
