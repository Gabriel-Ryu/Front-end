<template>
        <input type="text" id="textbox-nome" class="textbox-nome" placeholder="Nome" @focus="escrevendo"  @blur="naoEscrevendo">
</template>
<script>
export default {
    methods:{
        escrevendo(){
            document.getElementById("textbox-nome").placeholder = '';
        },
        naoEscrevendo(){
            document.getElementById("textbox-nome").placeholder = "Nome";
        }
    }
}
</script>
<style scoped>
.textbox-nome{
    background-color: #666666;
    color: #ccccc9;
    position: absolute;
    top: 40%;
    height: 20%;
    width: 160%;
    font-family: 'Montserrat', sans-serif;
    font-size: 120%;
}

.textbox-nome::placeholder {
    color: #ccccc9;
    padding-left: 5px;
}
</style>