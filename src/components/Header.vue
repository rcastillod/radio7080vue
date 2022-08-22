<template>
    <header class="main-header">
        <BaseLogo/>
        <ContactList></ContactList>
    </header>
</template>

<script>
import ContactList from './ContactList.vue';

    export default {
        name: "header-component",
        components: { ContactList }
    }
</script>

<style lang="scss" scoped>
    .main-header {
        padding: 1.25rem 3.125rem;
        position: absolute;
        width: 100%;
        z-index: 2;
    }
</style>