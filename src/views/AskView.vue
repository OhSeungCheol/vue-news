<template>
    <div>
        <div v-for="(ask, index) in this.$store.state.asks" v-bind:key="index">{{ask.title}}</div>
    </div>
</template>

<script>
export default {
    created() {
        this.$store.dispatch('FETCH_ASKS');
    }
}
</script>

<style>

</style>