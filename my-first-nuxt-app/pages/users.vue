<template>
    <div>
    <input type="text" v-model="userId">
    <button @click="onLoadUser">Load User</button>
    <nuxt-child/>
</div>
</template>


<script>
import Header from '~/components/Header.vue'
export default {
    
    data(){
        return{
            userId: ''
        }
    },
    methods:{
        onLoadUser(){
            this.$router.push('/users/'+this.userId);
        }
    },
    layout:'users'
}
</script>

<style scoped>
    
</style>