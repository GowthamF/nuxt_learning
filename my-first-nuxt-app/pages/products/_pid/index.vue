<template>
    <h2>The Product Id is {{$route.params.pid}}</h2>
</template>

<script>
export default {
    validate(data){
        console.log(data);
        return true;
    }
}
</script>