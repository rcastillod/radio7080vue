<template>
    <ul class="social-wrapper flex" role="list">
        <li v-for="(social, index) in socials" :key="index">
            <BaseLink :to="social.socialUrl">
                <BaseIcon :name="social.socialName"></BaseIcon>
            </BaseLink>
        </li>
    </ul>
</template>

<script>

    export default {
    data() {
        return {
            socials: [
                { socialName: "facebook", socialUrl: "https://www.facebook.com/" },
                { socialName: "instagram", socialUrl: "https://www.instagram.com/" },
            ]
        };
    }
}
</script>

<style lang="scss" scoped>

</style>