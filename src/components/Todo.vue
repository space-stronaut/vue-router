<template>
    <div>
        <form @submit="submit">
            <input/>
        </form>
    </div>
</template>

<script>
    export default{
        name : "Todo",
        data() {
            return {
                key: "value"
            }
        },
        methods: {
            submit(e) {
                e.preventDefault()
            }
        },
    }
</script>

<style scoped>

</style>