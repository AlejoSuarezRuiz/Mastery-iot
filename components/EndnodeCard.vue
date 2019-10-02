<template>
    <div class="main">
        <div class="card-head">
            <div class="card-title">{{ type }}</div>
            <span class="card-divider"></span>
        </div>
        <div class="endnode-content">
            <div class="endnode-data">
                <display-data :measure="measure">
                    {{ measure }}
                </display-data>
            </div>
            <div class="endnode-description">
                <div class="endnode-text">
                    <span style="display: flex;">Estado de conexión: <strong class="status">{{ conectionStatus }}</strong> </span>
                    <span>El limite configurado para la balanza es de {{ maxWeight }} Kg.</span>
                </div>
                <div class="button-action" style="height: auto">
                    <!-- <button v-on:click="changeData">Guardar</button> -->
                    <button v-on:click="connectWS"> Connect </button>
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
            conectionStatus:'Esperando',
            maxWeight:50,
            measure:0
        }
    },
    methods: {
        changeData: function() {
            this.measure += 1;
        },
        connectWS: function() {
            try{
                this.conectionStatus = "Estable";
                const sock_recv = new WebSocket('ws://68.183.149.80:5000/get_data')
                console.log("Connected!");
                console.log(sock_recv);
                sock_recv.addEventListener("message", function(event) {
                    //console.log(event.data); 
                    //console.log(parseInt(event.data)); 
                    this.measure = parseInt(parseFloat(event.data)*100/33000);
                }.bind(this));
                console.log("listener added!!");
            } catch {
                console.log("Failed to establish connection!! D:")
            }
        }
    }
}
</script>