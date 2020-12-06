<script>
  // import AudioPlayer from './components/AudioPlayer.svelte';
  let src = "image/myImages.png";
  // let icon= 'image/icon-img.png';
  let information = "my images portfolio";
</script>

<style>
  @media only screen and (max-width: 600px) {
    :global(body) {
      font-family: "Spartan", sans-serif;
      margin: auto;
    }
    .container {
      text-align: center;
      background-color: rgb(250, 250, 250);
      border-radius: 10px;
      box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.171);
    }

    img {
      width: 100px;
      border-radius: 100px;
    }

    h2.tentang_saya {
      font-weight: bold;
      text-transform: capitalize;
      font-family: "Spartan", sans-serif;
    }

    p.content_tentang {
      font-size: 14px;
      color: #525252;
    }

    a.button {
      background-color: #ec5858;
      color: white;
    }
  }

  @media only screen and (min-width: 1200px) {
    @import url("https://fonts.googleapis.com/css2?family=Spartan&display=swap");

    :global(body) {
      font-family: "Spartan", sans-serif;
      margin: auto;
    }

    .container {
      text-align: center;
      background-color: rgb(250, 250, 250);
      border-radius: 10px;
      box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.171);
      max-width: 50%;
    }

    img {
      width: 200px;
      border-radius: 100px;
    }

    h2.tentang_saya {
      font-weight: bold;
      text-transform: capitalize;
      font-family: "Spartan", sans-serif;
    }

    p.content_tentang {
      font-size: 20px;
      color: #525252;
    }

    a.button {
      background-color: #ec5858;
      color: white;
    }
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

<svelte:head>
  <title>Hai, Aku Fauzi Aku Seorang IT Support</title>
  <link rel="stylesheet" href="style.css" />
  <link rel="stylesheet" href="skeleton.css" />
</svelte:head>

<section>
  <div class="container">
    <div class="img"><img {src} alt={information} class="profile" /></div>

    <div class="content">
      <h2 class="tentang_saya">Tentang saya</h2>
      <p class="content_tentang">
        Hai, saya fauzi🖐. Saya mahasiswa di Universitas Bina Sarana Informatika
        mengambil jurusan Teknologi Komputer dan saat ini sudah berjalan di
        Semester 5. Hobi saya mendesain, bermain bulu tangkis, futsal, jika ada
        waktu saya bermain games 😅
      </p>
      <a class="button" href="https://dribbble.com/iamfauzi">Go my dribbble</a>

      <!-- <AudioPlayer  src="voice.mp3" /> -->
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
