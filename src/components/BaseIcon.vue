<template>
    <div class="icon-wrapper" v-html="svg"></div>
</template>

<script>
import feather from  'feather-icons'

    export default {
        props: {
            name: String,
            width: {
                type: [Number, String],
                default: 24
            },
            height: {
                type: [Number, String],
                default: 24
            },
        },
        computed: {
            svg() {
                return feather.icons[this.name].toSvg({
                    class: "icon",
                    width: this.width,
                    height: this.height,
                })
            }
        }
    }
</script>

<style lang="scss" scoped>
    .icon-wrapper {
        display: inline-flex;
        align-items: center;
        gap: 6px;
        color: var(--color-light);
        font-size: 1rem;
        font-weight: var(--fw-bold);
    }
    .icon {
        stroke: currentColor;
        stroke-width: 2;
        stroke-linecap: round;
        stroke-linejoin: round;
        fill: none;
    }
</style>