<template>
    <BaseLink class="contact-link flex" :to="linkUrl">
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
    .contact-link {
        align-items: center;
        color: var(--color-light);
        font-size: 1.125rem;
        text-decoration: none;
    }
</style>