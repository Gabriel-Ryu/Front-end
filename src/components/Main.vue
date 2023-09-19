<template>
    <div class="main-container">
        <li><Fotinho/></li>
        <li><Textbox/></li>
    </div>
</template>
<script>
import Fotinho from './Fotinho.vue'
import Textbox from './Textbox.vue'
export default{
  components: { Textbox,Fotinho },
  

}
    Fotinho
</script>
<style scoped>
.main-container{
    height: 50%;
    width: 100%;
    display:flex;
    align-items: center;
}

.main-container li{
    display: inline-block;
    width: 30%;
    height: 65%;
    position: relative;
    padding: 2%;
}
</style>