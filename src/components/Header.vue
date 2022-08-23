<template>
    <header class="main-header">
        <div class="container">
            <div class="header-wrapper flex">
                <BaseLogo/>
                <div class="flex">
                    <ContactList></ContactList>
                    <div class="vertical-spacer"></div>
                    <BaseSocialList></BaseSocialList>
                </div>
            </div>
        </div>
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
    .header-wrapper {
        justify-content: space-between;

        & > div {
            align-items: center;
        }
    }
    .vertical-spacer {
        background-color: var(--color-light);
        height: 50%;
        width: 1px;
    }
</style>