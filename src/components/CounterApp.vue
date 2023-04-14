<template >
    <div>
        <h1>CounterApp by Vue Js</h1>
    </div>
    <div>
        <h3>{{ count }}</h3>
    </div>
    <div class="bclass">
        <button @click="increment">+</button>
        <button @click="decrement">-</button>
    </div>
</template>
<script>
export default {
    data(){
        return {
            count:0
        }
    },
    methods: {
        increment(){
            this.count++
        },
        decrement(){
            this.count--
        }
    },
    
}
</script>
<style>
    h3{
        font-size: 50px;
    }
    button{
        padding: 15px;

    }
    .bclass{
        display: flex;
        justify-content: center;
        gap: 50px;
        background-color: transparent;
        border-radius: 30;
        /* padding: 30px; */

    }

</style>