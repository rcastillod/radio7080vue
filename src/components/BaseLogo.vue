<template>
    <div class="logo">
        <router-link to="/">
            <img src="../assets/logo.svg" alt="Radio 7080">
        </router-link>
    </div>
</template>

<script>
    export default {
        name: 'logo-component'
    }
</script>

<style lang="scss" scoped>
.logo img {
    width: 12.5rem;
}
</style>