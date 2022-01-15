<script>
	import Router from 'svelte-spa-router';
	import active from 'svelte-spa-router/active'
	import Home from './Home.svelte';
	import News from './News.svelte';
	import Login from './Login.svelte';
	const yr = new Date().getFullYear();
	const objs =[{title:'tunderbolt:our new templating language',src:'https://scontent.fcok10-1.fna.fbcdn.net/v/t39.8562-6/236059786_985111022325691_1310544145856897747_n.jpg?_nc_cat=103&ccb=1-5&_nc_sid=6825c5&_nc_ohc=uoXg69lmWeMAX_eaG99&_nc_ht=scontent.fcok10-1.fna&oh=00_AT8kZ_XwIsSbp8b8UHDqNsdS01FDAZza-lO54VnzlCEJUw&oe=61C87302'}]
	
</script>
<svelte:head>
	<link href="https://unpkg.com/tailwindcss@^1.0/dist/tailwind.min.css" rel="stylesheet">
</svelte:head>
<main>
	<div>
		<h2 class="logo">EventCircle</h2>
		<p class="subtitle">alpha version</p>
	</div>	
	<header>
		
		<nav>
			
		<a href="/" use:active>home</a>
		<a href="/#/news" use:active={'/news'}>news</a>
		<a href="/#/login" use:active={'/login'}>login</a> 
		</nav>
	</header>
	<Router routes={{
		'/':Home,
		'/news/':News,
		'/login/':Login,

	}}/>

	<footer style="background-color: black;height:350px;">
	  <div style="display:flex;flex-direction:row; justify-content:space-around;">
		  <div style="display: flex; flex-direction:column;">
			  
			<span><a href="https://github.com/mellofordev/eventCircle">Github</a></span>
			<span>Donate</span>
			<span>Credits</span>
		  </div>
		  <div style="display: flex; flex-direction:column;">
			  <p>Image Credits</p>
			  <p>Privacy Policy</p>
			  <p>Report</p>
			  <p>Bug Bounty</p>
		  </div>
	  </div>
	  <p style="text-align: center; color:blanchedalmond;padding-top:34px;">(c) {yr} sreedhar k.s </p><br>
	  <a href="#mit" style="text-align:center;"> MIT License</a>
	</footer>
</main>
<style>
	
	main{
		width: auto;
		background-color:rgb(18, 18, 18);
		color:whitesmoke;
		
	}
	
	
	header{
		background-color:rgb(18, 18, 18);
		flex-direction:row;
		width:100%;
		height:50px;
		position:sticky;
		top:0;
		z-index:999;
		padding-top:0px;
		
		
	}

	.logo{
		font-size:20px;
		font-family: sans-serif;
		padding-left: 35px;
		padding-right:30px;
		width:100%;
		background-color: rgb(32, 32, 32);
		background-attachment:scroll;
		color:white;
		
	}

	.subtitle{
		font-size: 15px;
		background-color:rgb(32,32,32);
		padding-left:10%;
		color: white;
	}
	nav{
		padding:0;
		margin:0;
		flex-direction: row;
		align-items: center;
		justify-content: center;
		display:flex;
		top:0;
		
	}
	:global(a.active){
		color:rgb(65, 209, 142);
		
	}
	:global(a.inactive){
		color:white;
	}
	a{
		font-size: 19px;
		
		font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
	    margin-left: 33px;
		padding-top:10px;
		border-radius: 15px;
		text-align: center;
		margin-right:33px;
	}

</style>
