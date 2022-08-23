<template>
    <ul class="list-wrapper flex" role="list">
        <li>
            <ContactLink 
                linkIcon="phone"
                linkUrl="https://wa.link/3m1tpl"
                linkName="+56 9 1234 5678">
            </ContactLink>
        </li>
        <li>
            <ContactLink 
                linkIcon="mail"
                linkUrl="mailto:contacto@radio7080.cl"
                linkName="contacto@radio7080.cl">
            </ContactLink>
        </li>
    </ul>
</template>

<script>
import ContactLink from '@/components/ContactLink.vue';

    export default {
        components: {
            ContactLink,
        },
        props: {
            layout: {
                type: String,
                default: 'horizontal'
            }
        },
    }
</script>

<style lang="scss" scoped>
    .list-wrapper {
        align-items: center;
    }
</style>