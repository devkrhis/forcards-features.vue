<template>
    <div id="TeamBuilder">
        <h2> Team Builder </h2>
        <h4> Criar e fortalecer as relações entre pessoas de um mesmo grupo, no contexto corporativo</h4>
        <div class="icon">
            <svg-icon type="mdi" :path="path"></svg-icon>
        </div>

    </div>
    
</template>

<script>
import SvgIcon from '@jamescoyle/vue-icon';
import { mdilFlash } from '@mdi/light-js';
export default {
    components: {
        SvgIcon
    },
    data(){
        return {
            path: mdilFlash,
        }
    }
    
}
</script>

<style scoped>
#TeamBuilder {
    border: 3px solid rgb(255, 255, 255);
    box-shadow: rgba(0, 0, 0, 0.19) 0px 10px 20px, rgba(0, 0, 0, 0.23) 0px 6px 6px;
    border-top: 3px solid palevioletred;
    width: 350px;
    height: 200px;
    padding-left: 15px;
    margin-right: 20px;
    padding-top: 10px;
}

#TeamBuilder h4 {
    color: rgba(167, 165, 165, 0.884);
}

.icon {
    padding-left: 290px;
    padding-top: 70px;
}

</style>