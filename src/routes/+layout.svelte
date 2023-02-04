<script>
	import '../app.css';
	import Header from './Header.svelte';
	import Footer from './Footer.svelte';
	
</script>

<svelte:head>
	<title>Aditya Raj | Blog</title>
	<!-- <link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /> -->
	
	<!-- <link href="https://fonts.googleapis.com/css2?family=Open+Sans&display=swap" rel="stylesheet" />
	<link href="https://fonts.googleapis.com/css2?family=Ubuntu+Mono&display=swap" rel="stylesheet" />
	<link href="https://fonts.googleapis.com/css2?family=Roboto+Mono&display=swap" rel="stylesheet" />

	<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono&display=swap" rel="stylesheet">

	<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" /> -->
</svelte:head>

<div class="app pt-4 px-8 2xl:px-40 2xl:pt-8">
	<Header />

	<main>
		<slot />
	</main>

	<Footer />
</div>
