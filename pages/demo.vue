<template>
	<main>
		<div class="demo-content" style="height: 100%;">
			<div class="demo">
				<endnode-card />
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
		<!-- <div class="demo-slide">
		</div> -->
	</main>
</template>

<style>

</style>

<script>
import EndnodeCard from '@/components/EndnodeCard.vue'
export default {
	data(){
		return {
			measure: 50
		};
	},
	components:{
		EndnodeCard,
	}

}
</script>