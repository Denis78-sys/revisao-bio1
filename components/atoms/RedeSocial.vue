<!-- eslint-disable vue/require-prop-types -->
<template>
    <a :href="url" target="_blank" > <img class="rede-social" :src="require(`@/assets/images/${logo}`)" :alt="titulo" :title="titulo"></a>
   
</template>

<script>
export default {
    props: {
        // eslint-disable-next-line vue/require-prop-types
        url:{
            required: true
        },
        // eslint-disable-next-line vue/require-prop-types
        titulo:{
            required: true
        },
        // eslint-disable-next-line vue/require-prop-types
        logo:{
            required: true
        }
    }


}
</script>

<style scoped>

img{
    width: 40px;
    
}
@media (max-width: 767px){
    img{
        width: 26px;
         height: auto;
    }
}
</style>