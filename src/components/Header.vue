<template>
    <header>
        <h1>{{ job }}</h1>
        <h2>{{ name }}</h2>
    </header>
</template>
<!----------Template / Script---------->
<script>
    export default {
        name: 'Header',
        data() {
            return {
                job: 'DEVELOPPEUR WEB',
                name: 'Fabio R. LOPES',
            }
        },
    }
</script>
<!----------Script / Style---------->
<style scoped>
    header {
        position: relative;
        overflow: hidden;
        height: 180px;
        width: 60%;
        min-width: 900px;
        margin: 20px auto 0 auto;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        border: 1px solid white;
        border-bottom: none;
        border-radius: 10px 10px 0 0;
    }

    header, h1, h2 {
        transition-duration: 250ms;
        transition-property: all;
    }

    h1 {
        line-height: 1em;
        font-size: 5em;
        letter-spacing: 18px;
        margin-right: -18px;
        cursor: default;
    }

    h2 {
        font-size: 3em;
        letter-spacing: 8px;
        margin-right: -8px;
        cursor: default;
    }

    header:hover h1 {
        letter-spacing: 4px;
        margin-right: -4px;
    }

    header:hover h2 {
        letter-spacing: 2px;
        margin-right: -2px;
    }
</style>