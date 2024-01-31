<template>
  <button class="botao" :style="{ backgroundColor: corDoBotao, color: corDoTexto }" @click="clicou()">{{ texto }}</button>
</template>

<script>
export default {
    props: {
        texto: {
            type: String,
            default: 'Clique aqui',
        },
        corDoBotao: {
            type: String,
            default: 'white',
        },
        corDoTexto: {
            type: String,
            default: 'black',
        }
    },
};
</script>

<style>
.botao {
    font-size: 16px;
    height: 30px;
}
</style>
