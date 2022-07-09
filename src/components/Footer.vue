<template>
    <footer>
        <h4>Coded with ❤️ by Fabio R. LOPES</h4>
    </footer>
</template>
<!----------Template / Script---------->
<script>
export default {
    name: 'Footer',
}
</script>
<!----------Script / Style---------->
<style scoped>
    footer {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 60%;
        min-width: 900px;
        height: 60px;
        margin: 0 auto;
        border-radius: 0 0 10px 10px;
		border: 1px solid var(--front);
        border-top: none;
    }

    h4 {
        font-size: 1.1em;
        font-style: italic;
        letter-spacing: 1px;
    }

    @media screen and (max-width: 940px) {
        footer {
            width: 95%;
            min-width: 300px;
        }
    }

</style>