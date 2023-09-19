<template>
  <div class="footer-container">
        <BotaoContinuar/>
        <BotaoCancelar/>
    </div>
</template>
<script>
import BotaoCancelar from './BotaoCancelar.vue';
import BotaoContinuar from './BotaoContinuar.vue';
export default{
    components: { BotaoCancelar, BotaoContinuar }
}

</script>
<style scoped>
.footer-container {
    height: 10%;
    width: 100%;
    display: flex;
    align-items: flex-start;
    justify-content: space-around;
    
}
</style>