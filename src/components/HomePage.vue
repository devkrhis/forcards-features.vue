<template>
    <div class="controlAllItems">
        <p> Reliable, efficient delivery </p>
        <p> Powered by technology </p>
        <p> these cards refer to features for a better presentation of the page </p>
        <div class="alignItems">
            <SupervisorCard/>
            <SvgIcon type="mdi" :path="path"></SvgIcon>
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
import SvgIcon from "@jamescoyle/vue-icon";
import { mdiWalletOutline } from '@mdil/js';


export default {
    components: {
        SupervisorCard,
        TeamBuilder,
        KarmaCard,
        CalculatorCard,
        SvgIcon

    },
    data(){
        return {
            path: mdiWalletOutline,
        }
    },

    
}
</script>

<style scoped>

.controlAllItems p{
    display: flex;
    justify-content: center;
    
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