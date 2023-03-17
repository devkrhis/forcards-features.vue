<template>
    <div id="supervisor">
        <h2> Supervisor </h2>
        <h4> Um supervisor supervisiona o trabalho e desempenho. </h4>
        <div class="icon">
            <svg-icon type="mdi" :path="path"></svg-icon>
        </div>

    </div>
    
</template>

<script>

import SvgIcon from '@jamescoyle/vue-icon';
import { mdilEye } from '@mdi/light-js';

export default {
    props: ['nome'],
    components: {
        SvgIcon
    },
    data(){
        return {
            path: mdilEye
        }
    }
    
}
</script>

<style scoped>

#supervisor {
    border: 3px solid rgb(255, 255, 255);
    box-shadow: rgba(0, 0, 0, 0.19) 0px 10px 20px, rgba(0, 0, 0, 0.23) 0px 6px 6px;
    border-top: 3px solid rgb(116, 170, 250);
    width: 350px;
    height: 200px;
    padding-left: 15px;
    margin-right: 20px;
    padding-top: 10px;

}

#supervisor h4 {
    color: rgba(167, 165, 165, 0.884);
}

.icon {
    padding-left: 290px;
    padding-top: 70px;
}

</style>