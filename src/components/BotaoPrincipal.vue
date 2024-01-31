<template>
  <button class="botao" :style="{ backgroundColor: corDoBotao, color: corDoTexto }" @click="clicou()">{{ texto }}</button>
</template>

<script>
export default {
    data(){
        return {
            corDoBotao: 'green'
        }
    },
    
    props: {
        texto: {
            type: String,
            default: 'Clique aqui',
        },
        
        corDoTexto: {
            type: String,
            default: 'black',
        }
    },
    methods:{
        clicou(){
            this.corDoBotao = 'red'
        }
    }
};

</script>

<style>
.botao {
    font-size: 16px;
    height: 30px;
}
</style>
