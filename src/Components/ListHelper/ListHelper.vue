<template>
    <div>

        <slot name="listItem"></slot>

        I am a helper person

       <slot name="para"></slot>
        <slot name="other">Loading.....</slot>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>

</style>