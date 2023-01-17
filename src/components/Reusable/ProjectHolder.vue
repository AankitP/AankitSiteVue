<template>
    <slot></slot>
</template>

<script>
export default {
  name: "ProjHolder",
  setup() {},
};
</script>

<style>

    .allHolderProj{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        margin: 5%;
    }

    .textHolderProj{
        display: flex;
        flex-direction: column;
        text-align: left;
        width: 50%;
    }

    h5{
        margin-left: 1rem;
    }

    .ProjImg {
        aspect-ratio: "1.33" !important;
        max-width: 15%;
        max-height: 15%;
        border-radius: 1rem;
        margin-right: 5%;
    }

</style>