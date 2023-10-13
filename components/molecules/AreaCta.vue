<template>
    <div>
       <ul class="area-cta">
        <li v-for="tituloCta in titulosCta" :key="tituloCta.id" class="item"><Cta :titulo-descricao="tituloCta.descricao" :link-zap="tituloCta.urlLink"/></li>
       </ul>
    </div>
</template>

<script>
export default {
    data(){
        return {titulosCta:[{id: 1, descricao: 'Desenvolvimento web', urlLink: 'https://web.whatsapp.com/'},
        {id: 2, descricao: 'Flyer para evento', urlLink: 'https://web.whatsapp.com/'},
        {id: 3, descricao: 'Suporte em TI', urlLink: 'https://web.whatsapp.com/'},
        {id: 4, descricao: 'Contato WhatsApp', urlLink: 'https://web.whatsapp.com/'}
        ]}
    }
}
</script>

<style scoped>
li{
    list-style: none;
}
.area-cta{
    display: grid;
    grid-gap: 24px;
}
</style>