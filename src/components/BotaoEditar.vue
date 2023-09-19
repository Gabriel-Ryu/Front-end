<template>
    <div class="container-btn-editar" @mouseover="mostraBotao" @mouseleave="escondeBotao" >
        <input type="button" value="Edit" class="material-symbols-outlined" ref="botao-editar" >
    </div>
</template>
<script>
export default {
    data(){
        return{
            mostrar_botao:false,
        }
    },
    methods:{
        mostraBotao(){
            document.querySelector("input").style.visibility = 'visible';
            document.querySelector("input").style.opacity = '1';
        },
        escondeBotao(){
            document.querySelector("input").style.visibility = 'hidden';
            document.querySelector("input").style.opacity = '0';
        }
    }
}
</script>

<style scoped>
.material-symbols-outlined {
background-color: black;
color: aliceblue;
border-color: aliceblue;
border-style: solid;
width: 50%;
height: 50%;
border-radius: 100%;
border-width: 5px;
margin: 25%;
cursor: pointer;
transition: 0.5s;
visibility: hidden;
font-size: 60px;
font-variation-settings:
  'FILL' 1,
  'wght' 200,
  'GRAD' 0,
  'opsz' 20
}

.material-symbols-outlined:hover {
    transition: 0.5s;
}
.container-btn-editar{
    position: absolute;
    width: 90%;
    height: 90%;
    display: flex;
    justify-content: center;
    background-color: rgba(0, 0, 0, 0);
    transition: 0.5s;
}

.container-btn-editar:hover{
    background-color: rgba(0, 0, 0, 0.5);
    transition: 0.5s;
    
}
</style>