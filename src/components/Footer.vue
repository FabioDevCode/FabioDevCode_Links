<template>
    <footer>
        <h3>
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><path d="M416 352c-8.188 0-16.38-3.125-22.62-9.375L224 173.3l-169.4 169.4c-12.5 12.5-32.75 12.5-45.25 0s-12.5-32.75 0-45.25l192-192c12.5-12.5 32.75-12.5 45.25 0l192 192c12.5 12.5 12.5 32.75 0 45.25C432.4 348.9 424.2 352 416 352z"/></svg>
            PROJECTS LINKS
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><path d="M416 352c-8.188 0-16.38-3.125-22.62-9.375L224 173.3l-169.4 169.4c-12.5 12.5-32.75 12.5-45.25 0s-12.5-32.75 0-45.25l192-192c12.5-12.5 32.75-12.5 45.25 0l192 192c12.5 12.5 12.5 32.75 0 45.25C432.4 348.9 424.2 352 416 352z"/></svg>
        </h3>
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
        overflow: hidden;
        width: 60%;
        min-width: 900px;
        height: 60px;
        margin: 0 auto 30px auto;
        border-radius: 0 0 10px 10px;
		border: 1px solid var(--front);
        border-top: none;
    }

    h3 {
        display: flex;
        justify-content: center;
        align-items: center;
        overflow: hidden;
        flex-wrap: nowrap;
        width: 100%;
        align-self: center;
        font-size: 1.4em;
        padding: 15px 0;
        border-top: none;
    }

    h3 svg {
        height: .9em;
        margin: 5px 15px 0 15px;
        fill: var(--front);
    }

    @media screen and (max-width: 940px) {
        footer {
            width: 95%;
            min-width: 300px;
        }

        h3 {
            font-size: 1.2em;
        }

        h3 svg {
            height: .7em;
        }
    }
</style>