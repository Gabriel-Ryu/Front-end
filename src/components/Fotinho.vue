<template>
    <div class="container-fotinho" >
        <img :src="avatar" :alt="descricao" class="fotinho">
        <BotaoEditar/>
    </div>
</template>
<script>
import BotaoEditar from './BotaoEditar.vue';
export default{
    components:{BotaoEditar},
    name:'Picture',
    data(){
        return{
            avatar:"/img/fotinho.png",
            descricao:"Fotinho"
        }
    },
}
</script>
<style scoped>
.container-fotinho{
    width: 100%;
    height: 100%;
    padding: 0%;
    border: 0;
    display: flex;
    align-items: flex-start;
    cursor: default;
}

.fotinho{
    width: 100%;
    height: 100%;
    border-radius: 2%;
}


</style>