<template>
    <div id="supervisor">
        <h2> Supervisor </h2>
        {{ path }}

    </div>
    
</template>

<script>

export default {
    props: ['path'],
    components: {
    },
    data(){
        return {
        }
    }
    
}
</script>

<style scoped>

#supervisor {
    border: 3px solid rgb(255, 255, 255);
    box-shadow: rgba(0, 0, 0, 0.19) 0px 10px 20px, rgba(0, 0, 0, 0.23) 0px 6px 6px;
    border-top: 3px solid rgb(116, 170, 250);
    width: 250px;
    height: 200px;
    padding-left: 15px;
    margin-right: 20px;

}

</style>