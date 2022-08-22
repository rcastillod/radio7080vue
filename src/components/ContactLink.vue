<template>
    <BaseLink :to="linkUrl">
        <BaseIcon :name="linkIcon" />
        {{ linkName }}
    </BaseLink>
</template>

<script>
    export default {
        props: {
            linkIcon: String,
            linkName: {
                type: String,
                required: true
            },
            linkUrl: {
                type: String,
                required: true
            }
        },
    }
</script>

<style lang="scss" scoped>

</style>