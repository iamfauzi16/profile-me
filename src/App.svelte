<script>
	let src= 'image/myImages.png';
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
}

h2.tentang_saya {
	font-family: 'Staatliches', cursive;
}

p.content_tentang {
	font-size: 16px;
	color: #393e46;
	text-align: left;
}



</style>

<section>
	<div class="container">
		<div class="row">
			<div class="five columns">
				<img src={src} alt={information} class="profile">
			</div>
			<div class="seven columns">
				<h2 class="tentang_saya">Tentang saya</h2>
				<p class="content_tentang">Lorem ipsum dolor sit amet consectetur adipisicing elit. Repudiandae voluptatibus magni neque similique natus dolore accusantium accusamus ipsam iusto! Nisi accusamus totam nulla blanditiis quisquam nam, unde rem numquam inventore voluptatem laudantium architecto, eaque consequuntur obcaecati expedita fuga a repellat neque. Corrupti sed, magni nam iure doloribus optio itaque, sapiente voluptatum ad non delectus veniam iusto praesentium id asperiores? Omnis voluptatibus autem similique doloribus velit ipsum, distinctio, error officia consequatur dolor atque rem sed architecto, dolores esse nisi? Cumque corporis rem, assumenda dolor a repudiandae consectetur impedit cum dolores molestiae. Saepe, sequi sapiente! Voluptatibus provident quae, enim distinctio harum nulla?</p>
			</div>
		</div>
	</div>
</section>

