<template>
	<main>
		<div class="demo-content">
			<endnode-card :mesaure="mesaure" />
			<div class="demo-introduction">
				<h4>Dashboard de adquisición </h4>
				<p>
					Gracias a la capacidad de conexión inalámbrica que presenta la tarjeta, se pueden construir dashboards que se encargan de mostrar la información entregada por la misma. Además, se puede interactuar direactamente con una base de datos y almacenar los valores más importantes. 
				</p>
			</div>
		</div>
		<div class="demo-slide">
			
		</div>
	</main>
</template>

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