<template >
    <div>
        <!-- <h2>Name: {{ name  }}</h2> -->
        <!-- <h2>Data: {{ getData()  }}</h2> -->
        <h2>Name: {{ getData().name }}</h2>
        <h2>Data: {{ getData().age }}</h2>
        <button @click="ageChange()">change age</button>
        <button v-on:click="test()">Click Me</button>
        <div>
            <input type="text" v-model="datas">
            <h3>{{ datas }}</h3>
        </div>

    </div>
</template>
<script>
export default {
    data() {
        return {
            name: "sanmay",
            age: 25,
            datas: 0
        }
    },
    methods: {
        getData() {
            return {
                name: this.name,
                age: this.age,
            }
        },
        ageChange() {
            this.age++
        },
        test() {
            alert(this.age++)
        }
    },

}
</script>
<style ></style>