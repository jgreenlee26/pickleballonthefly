<template>
    <button class="jdz-btn">{{ text }}</button>
</template>
<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
    name: "JdzBtn",
    props: {
        text: {
            type: String,
            default: "Button",
        },
    },
    setup(props) {
        return {
            text: props.text,
        };
    },
});
</script>
<style scoped>
.jdz-btn {
    display: flex;
    flex-direction: row;
    max-width: 157px;
    justify-content: flex-start;
    align-items: flex-start;
    border-radius: 15px;
    box-shadow: 0px 4px 4px 0px rgba(0, 0, 0, 0.25);
    padding-top: 26px;
    padding-right: 60px;
    padding-bottom: 26px;
    padding-left: 60px;
    border-color: rgba(0, 0, 0, 1);
    border-width: 1px;
    border-style: solid;
    background-color: rgba(15, 157, 88, 1);
    color: rgba(255, 255, 255, 1);
    font-size: 28px;
    letter-spacing: 0%;
    text-align: center;
    font-family: "Montserrat", sans-serif;
}
</style>
