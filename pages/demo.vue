<template>
	<main>
		<div class="demo-content">
			<div class="demo">
				<endnode-card :mesaure="mesaure" />
			</div>
			<div class="demo-introduction">
				<div class="introduction-title">
					Dashboard de adquisición
				</div>
				<span class="divider"></span>
				<div class="introduction-body">
					Gracias a la capacidad de conexión inalámbrica que presenta la tarjeta, se pueden construir dashboards que se encargan de mostrar la información entregada por la misma. Además, se puede interactuar direactamente con una base de datos y almacenar los valores más importantes. 
				</div>
			</div>
		</div>
		<div class="demo-slide">
		</div>
	</main>
</template>

<style>
	.demo-content {
		height: 70vh; 
		display: flex;
		flex-direction: row;
	}

	.demo {
		width: 45vw;
		display:flex;
		align-items: center;
		justify-content: center;
	}

	.demo-introduction {
		width: 45vw;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}

	.introduction-title {
		font-family: 'Rasa';
		font-style: normal;
		font-weight: bold;
		font-size: 36px;
		line-height: 44px;
		color: #475071;
	}

	.introduction-body {
		font-family: 'Rasa';
		font-style: normal;
		font-weight: normal;
		font-size: 28px;
		line-height: 34px;
		text-align: center;
		color: #475071;
		width: 75%;
	}

	.divider {
		background-color: #475071;
		width: 55%;
		height: 3px;
		margin-bottom: 25px;
		margin-top: 5px;
		border-radius: 3px;
	}

	.demo-slide {
		height: 30vh;
		background-color: #9FA9D0;
	}
</style>

<script>
import EndnodeCard from '@/components/EndnodeCard.vue'
export default {
	data(){
		return {
			mesaure: 25.8
		};
	},
	components:{
		EndnodeCard,
	}

}
</script>