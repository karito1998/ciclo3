<template>
    <div>    
        <div class = "card text-white bg-dark">
            <div class= "d-flex justify-content-center p-2">
                <img :src="member.image" alt="participante" height="250" width="250">
            </div>
        <div class = "card-body">
            <h5 class = "card-title"> {{member.nombre}} </h5>
            <p class = "card-text"> {{member.descripcion}} </p>
        </div>
        <div class = "card-footer">
            <small class="text-muted"> {{member.rol}}</small>
        </div>
    </div>
</div>
    
</template>

<script>
    export default {
        name: "TeamCard",
        props: ['member']
    }
</script>

<style scoped>

</style>
