<template>
    <div class="main">
        <div class="card-head">
            <div class="card-title">{{ type }}</div>
            <span class="card-divider"></span>
        </div>
        <div class="endnode-content">
            <div class="endnode-data">
                <display-data>
                    {{ mesaure }}
                </display-data>
            </div>
            <div class="endnode-description">
                <div class="endnode-text">
                    <span style="display: flex;"><p style="width: 70%">Estado de conexión: <strong class="status">{{ conectionStatus }}</strong> </p> </span>
                    <span>El limite configurado para la balanza es de {{ maxWeight }} Kg.</span>
                </div>
                <div class="button-action">
                    <button>Guardar</button>
                </div>
            </div>
        </div>
        
    </div>
</template>

<style>
    
</style>

<script>
import DisplayData from '@/components/DisplayData.vue'
export default {
    components:{
        DisplayData
    },
    data(){
        return{
            type:'Medición',
            conectionStatus:'Estable',
            maxWeight:50
        }
    },
    props:['mesaure']
}
</script>