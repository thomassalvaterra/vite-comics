<script>
import AppCard from './AppCard.vue'

export default {
	name: "AppJumbo",
	props: ["cards"],
	components: {
		AppCard
	}
}
</script>

<template>
	<div class="jumbotron"></div>
	<section id="bg-black">
		<main>
			<div id="cardsWrapper">
				<AppCard v-for="card in cards" :carta="card" />
			</div>
		</main>
		<section id="btn-section">
			<button id="btn"><b>LOAD MORE</b></button>
		</section>
	</section>
</template>

<style scoped>
.jumbotron {
	background-image: url(../assets/img/jumbotron.jpg);
	background-size: cover;
	height: 20rem;
	display: flex;
	align-items: center;
}

#bg-black {
	background-color: #222;
}

main {
	width: 1400px;
	margin: 0 auto;
	display: flex;
	align-items: center;
}

#cardsWrapper {
	display: flex;
	flex-wrap: wrap;
}

#btn-section {
	display: flex;
	justify-content: center;
}

#btn {
	background-color: rgb(52, 161, 235);
	color: white;
	padding: 20px;
	margin-bottom: 20px;
	width: 180px;
}
</style>