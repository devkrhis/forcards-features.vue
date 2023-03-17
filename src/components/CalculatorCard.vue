<template>
    <div id="Calculator">
        <h2> Calculator </h2>
        <h4> Em resumo, é a lei de causa e efeito atuante. A todo instante. </h4>
        <div class="icon">
            <svg-icon type="mdi" :path="path"></svg-icon>

        </div>

    </div>
    
</template>
<script>
import SvgIcon from '@jamescoyle/vue-icon';
import { mdiLaptop } from '@mdi/js';
export default {
    components: {
    SvgIcon
  },
  data() {
    return {
       path: mdiLaptop,
    }
  }
    
}
</script>

<style scoped>
#Calculator {
    border: 3px solid rgb(255, 255, 255);
    box-shadow: rgba(0, 0, 0, 0.19) 0px 10px 20px, rgba(0, 0, 0, 0.23) 0px 6px 6px;
    border-top: 3px solid blue;
    width: 350px;
    height: 200px;
    padding-left: 15px;
    padding-top: 10px;

}

#Calculator h4 {
    color: rgba(167, 165, 165, 0.884);
}


.icon {
    padding-left: 290px;
    padding-top: 70px;
}

</style>