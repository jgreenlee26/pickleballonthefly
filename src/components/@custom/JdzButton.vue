<template>
    <button
        class="jdz-button"
        :class="{ 'rounded': rounded }" 
        :disabled="disabled"
        :style="{ backgroundColor: color, color: textColor }"
    >
        <i v-if="icon" class="material-icons mr-2">{{ icon }}</i>
        <slot></slot>
    </button>
</template>
<script>
export default {
    name: "jdz-button",
    props: {
        disabled: {
            type: Boolean,
            default: false
        },
        color: {
            type: String,
            default: "#0F9D58"
        },
        icon: {
            type: String,
            default: ""
        },
        loading: {
            type: Boolean,
            default: false
        },
        rounded: {
            type: Boolean,
            default: true
        },
        shape: {
            type: String,
            default: "rectangle" // what other options?
        },
        textColor: {
            type: String,
            default: "white"
        }
    }
}
</script>
<style lang="scss">
.jdz-button {
    font-family: 'Poppins' "Poppins" Arial, serif;
    font-style: normal;
    font-weight: 700;
    font-size: 16px;
    line-height: 42px;
    padding: 8px 46px;
    display: flex;
    align-items: center;
    text-align: center;
}
.rounded {
    border-radius: 15px;
}
</style>