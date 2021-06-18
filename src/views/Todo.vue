<template>
    <div>
        <form v-on:submit="kirim">
            <input type="text" v-model="value"/>
            <button type="submit">Submit</button>
        </form>
        <ul 
        v-for="person in persons" 
        :key="person.id">
            <li>{{person}}</li>
        </ul>
    </div>
</template>

<script>
    export default{
        name : "Todo",
        data() {
            return {
                persons: [],
                value : ""
            }
        },
        methods: {
            kirim(e) {
                e.preventDefault()
                this.persons.push(this.value)
                this.value = ""
            }
        },
    }
</script>

<style scoped>

</style>