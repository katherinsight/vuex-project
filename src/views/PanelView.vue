<template>
    <div id="panel">
        현재 카운터의 값 : {{count}}
    </div>
</template>

<script>
    export default {
        computed: {
            count() {
                return this.$store.state.count
            }
        },
    }
</script>

<style>
    #panel {
        margin-bottom: 20px;
    }

</style>