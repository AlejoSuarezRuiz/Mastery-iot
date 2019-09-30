<template>
    <section>
        <strong>{{ type }}</strong>
        <div class="endnode-content">
            <display-data>
                {{ mesaure }}
            </display-data>
            <div class="endnode-text">
                <span>Estado de conexión: {{ conectionStatus }} </span>
                <span>El limite configurado para la balanza es de {{ maxWeight }} Kg</span>
            </div>
            <div class="button-action">
                <button>Guardar</button>
            </div>
        </div>
        
    </section>
</template>

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