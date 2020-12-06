<template>
    <div>
        <div class="card mb-3" style="width: 220px; height: 400px">
            <img class="card-img-top" :src="member.imagen" width="200px" height="200px" alt="miembro">
            <div class="card-body text-white bg-dark text-center">
                <p class="card-title">{{member.nombre}}</p>
                <p class="card-text">{{member.descripcion}}</p>
                <p class="card-text">id: {{member.codigo}}</p>
                <p class="card-text">Rol: {{member.rol}}</p>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "TeamCard",
        props: ['member'],
    }
</script>

<style scoped>

</style>
