<template>
    <a 
        v-if="isExternal" 
        :href="to"
        target="_blank"
        rel="noopener"
    ><slot/></a>
    <router-link v-else :to="to"><slot/></router-link>
</template>

<script>

    export default {
        name: 'base-link',
        props: {
            to: {
                type: String,
                required: true
            }
        },
        computed: {
            isExternal() {
                return typeof this.to === 'string' && this.to.startsWith('http')
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>