<template>
    <div class="controlAllItems">
        <h1> <p class="firstLine"> Reliable, efficient delivery </p> </h1> 
        <h1> <p> Powered by technology </p> </h1>
        <h4> <p> these cards refer to features for a better presentation of the page so we can show supervisor, team builder, karma and calculator </p> </h4>
        <div class="alignItems">
            <SupervisorCard :nome="nome"/>
            <div class="alignItemsColumn"> 
                <TeamBuilder/>
                <KarmaCard/>
            </div>
            <CalculatorCard/>
        </div>
    </div>
</template>

<script>
import SupervisorCard from './SupervisorCard.vue'
import TeamBuilder from './TeamBuilder.vue';
import KarmaCard from './KarmaCard.vue';
import CalculatorCard from './CalculatorCard.vue';


export default {
    components: {
        SupervisorCard,
        TeamBuilder,
        KarmaCard,
        CalculatorCard,

    },
    data(){
        return {
            nome: "Krhistopher"
        }
    },

    
}
</script>

<style scoped>
.controlAllItems p{
    display: flex;
    justify-content: center;
    
}

.controlAllItems h1{
    margin-top: 50px
}

.controlAllItems .firstLine{
    margin-bottom: -60px;
    color: rgba(167, 165, 165, 0.884);
}

.controlAllItems h4{
    color: rgba(167, 165, 165, 0.884);
    margin-bottom: 30px;
}

.controlAllItems .forLine{
    word-wrap: break-word;
    width: 650px;
    display: flex;
    align-items: center;

}

.alignItems {
    display: flex;
    align-items: center;
    justify-content: center;
}

.alignItemsColumn{
    display: flex;
    flex-direction: column;
}

</style>