<template>
    <kinesis-container perspective="1000">
        <kinesis-element id="card" :strength="-2000" type="depth">
            <kinesis-element class="title" :strength="-20" type="translate">
                <h1>FabioDevCode</h1>
            </kinesis-element>


        </kinesis-element>



    </kinesis-container>
</template>
<!---------- Template / Script ---------->
<script>
    export default {
        name: 'Card',
        data() {
            return {

            }
        },
        methods: {


        },
    }
</script>
<!---------- Script / Style ---------->
<style scoped>
    #card {
        position: relative;
        background: rgb(2,0,36);
        background: url('/abstract.webp');
        background-repeat: no-repeat;
        background-size: cover;
        height: 500px;
        width: 800px;
        border-radius: 25px;
        border: 1px solid grey;
        overflow: hidden;
    }

    .title {
        display: flex;
        justify-content: center;
        align-items: center;
        color: whitesmoke;
        mix-blend-mode: difference;
        height: 60px;
        width: 100%;
    }

    h1 {
        text-shadow: 10px 10px 20px rgba(18,18, 18, .5);
    }


</style>