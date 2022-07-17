<template>
    <kinesis-container>

        <kinesis-element id="card" :strength="40">
            <div class="bandeau">
                <h1>Développeur Web</h1>
            </div>

            <kinesis-element class="title" :strength="40">

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
        background: rgb(2,0,36);
        background: linear-gradient(-90deg, rgba(2,0,36,1) 0%, rgba(0,212,255,1) 100%);
        height: 540px;
        width: 840px;
        border-radius: 25px;
        overflow: hidden;
    }

    .bandeau {
        height: 50px;
        width: 100%;
        background-color:  rgb(2,0,36);
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .title {
        display: inline-block;
        background-color: teal;
    }


</style>