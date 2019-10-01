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
                    <span style="display: flex;"><p style="width: 70%">Estado de conexión: </p> <p class="status">{{ conectionStatus }}</p> </span>
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
    .main {
        background-color: #D7DEEA;
        border-radius: 10px;
        display:flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 400px;
        height: 500px;
    }
    
    .card-head {
        display: flex;
        flex-direction: column;
        width: 100%;
        justify-content: center;
        align-items: center;
        height: 20%;
    }

    .card-title {
        color: #4B5B85;
        margin: 10px 0px 0px 10px;
        font-family: 'Rasa';
        font-style: normal;
        font-weight: 600;
        font-size: 24px;
        line-height: 29px;
        width: 100%;
        text-align: left;
        margin-left: 50px;
    }

    .card-divider {
		background-color: #475071;
		width: 95%;
		height: 3px;
        margin-bottom: 25px;
		margin-top: 5px;
		border-radius: 3px;
	}

    .endnode-content {
        height: 80%;
        display: flex;
        flex-direction: column;
    }

    .endnode-text {
        display: flex;
        flex-direction: column;
        padding-left: 10%;
        padding-right: 10%;
        font-family: 'Rasa';
        font-style: normal;
        font-weight: normal;
        font-size: 24px;
        line-height: 29px;
        color:#4B5B85;
    }

    .endnode-text span {
        padding-top: 5%;
    }

    .status {
        color: #35AD33;
        font-family: Rasa;
        font-weight: bold;
    }

    .button-action button {
        background-color: #4B5B85;
        font-family: Rasa;
        font-style: normal;
        font-weight: bold;
        font-size: 48px;
        line-height: 58px;
        color: white;
        width: 280px;
        height: 65px;
        border-radius: 10px;
        box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
        border: none;
    }

    .button-action button:hover {
        width: 300px;
        height: 70px;
        font-size: 50px;
    }

    .endnode-data {
        height: 40%;
    }

    .endnode-description {
        height: 40%;
    }
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