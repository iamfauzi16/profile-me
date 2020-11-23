<script>
	import HeaderSatu from './components/HeaderSatu.svelte';
	import Content from './components/Content.svelte';
	import  {fly, fade} from 'svelte/transition';
	import Footer from './components/Footer.svelte';


	let isLoaded= false;

	setTimeout(function (){
		isLoaded = true;
	}, 2000);

	
</script>

<svelte:head>
	<link rel="stylesheet" href="nes.min.css">
	<!-- google font -->
	<link href="https://fonts.googleapis.com/css?family=Press+Start+2P" rel="stylesheet">
</svelte:head>

<style>
	.main {
		text-align: center;
		height: auto;
	}

	.container	{
		height: 300px;
		background-color: #e4e978;

	}
	.nes-btn {
		margin-top: 2em;
		color: white;
	}

	.a {
		background-color:#0f4c75;
	}

	.b {
		background-color:#00b7c2;
	}

	.c {
		background-color: #d54062;
	}

	.icon {
		margin-top: 1em;

	}


	/* Skills div */

	.skills {
		margin-top: 2em;
		margin-bottom: 3em;
	}
	
</style>

<div class="main">
	<HeaderSatu />
	<h2>Halo, bro</h2>
	<p>Selamat Datang silahkan kunjungi sosial media gue</p>
	<div class="container">
	{#if isLoaded}
		<div in:fly={{ y: 200, duration: 2000}} out:fade id="header">
			<a class="nes-btn a" href="https://www.facebook.com/ZigoongRev/">Facebook</a>
			<a class="nes-btn b" href="https://twitter.com/mhmmdfauzi_22">Twitter</a>
			<a class="nes-btn c" href="https://dribbble.com/iamfauzi">Dribbble</a>
			
			<div class="icon">
				<i class="nes-icon is-large heart"></i>
				<i class="nes-icon is-large heart"></i>
				<i class="nes-icon is-large heart"></i>
				<i class="nes-icon is-large is-half heart"></i>
			</div>
		</div>
		{/if}
	</div>


	<div class="skills">
		<h2>Skills</h2>
		<progress class="nes-progress" value="80" max="100"></progress>
		<Content skills={'Troubleshoot Hardware , Software PC Desktop atau Laptop'}/>
		
		<progress class="nes-progress" value="70" max="100"></progress>
		<Content skills={'Konfigurasi Mikrotik dan Hotspot'}/>

		<progress class="nes-progress" value="85" max="100"></progress>
		<Content skills={'Membuat User Interface Dengan Figma dan adobe XD'}/>
	</div>

	<Footer />
</div>