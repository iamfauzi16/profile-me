<script>
	// import AudioPlayer from './components/AudioPlayer.svelte';
	let src= 'image/myImages.png';
	// let icon= 'image/icon-img.png';
	let information = 'my images portfolio';
</script>

<svelte:head>
	<title>Hai, Aku Fauzi Aku Seorang IT Support</title>
	<link rel="stylesheet" href="style.css">
	<link rel="stylesheet" href="skeleton.css">
</svelte:head>


<style>
@import url('https://fonts.googleapis.com/css2?family=Red+Hat+Display&family=Staatliches&display=swap');


:global(body){
	font-family: 'Red Hat Display', sans-serif;
	
}

img {
	width: 200px;
	border-radius: 100px;

}

h2.tentang_saya {
	font-family: 'Staatliches', cursive;
}

p.content_tentang {
	font-size: 16px;
	color: #393e46;
	text-align: left;
}

a.button {
	background-color: #ec5858;
	color: white;
}

/* ul {
	text-align: center;
	padding: 40px;
	
}
li {
	display: inline-block;
	padding-right: 3em;
}

li img {
	width : 80px;
	
} */



</style>

<section>
	<div class="container">
		<div class="row">
			<div class="five columns">
				<img src={src} alt={information} class="profile">
			</div>
			<div class="seven columns">
				<h2 class="tentang_saya">Tentang saya</h2>
				<p class="content_tentang">Hai, saya fauzi🖐. Saya mahasiswa di Universitas Bina Sarana Informatika mengambil jurusan Teknologi Komputer dan saat ini  sudah berjalan di Semester 5. Hobi saya mendesain, bermain bulu tangkis, futsal, jika ada waktu saya bermain games 😅</p>
				<a class="button" href="https://dribbble.com/iamfauzi">Go my dribbble</a>

				<!-- <AudioPlayer  src="voice.mp3" /> -->
			</div>
		</div>
	</div>
</section>

<!-- <section>
	<div class="container">
		<div class="row">
			<ul class="icon">
				<li class="icon icon-1">
					<img src={icon} alt="" />
					<h4>Junior High School</h4>
					<p>SMP Pgri Depok 2 Tengah</p>
				</li>
				<li class="icon icon-2">
					<img src={icon} alt=""/>
					<h4>Senior High School</h4>
					<p>SMK Citra Negara</p>
				</li>
				<li class="icon icon-3">
					<img src={icon} alt=""/>
					<h4>University</h4>
					<p>Universitas Bina Sarana Informatika</p>
				</li>
			</ul>
		</div>
	</div>
</section> -->

