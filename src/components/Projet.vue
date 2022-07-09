<template>
    <main>
        <h3>
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><path d="M224 416c-8.188 0-16.38-3.125-22.62-9.375l-192-192c-12.5-12.5-12.5-32.75 0-45.25s32.75-12.5 45.25 0L224 338.8l169.4-169.4c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25l-192 192C240.4 412.9 232.2 416 224 416z"/></svg>
            PROJECTS LINKS
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><path d="M224 416c-8.188 0-16.38-3.125-22.62-9.375l-192-192c-12.5-12.5-12.5-32.75 0-45.25s32.75-12.5 45.25 0L224 338.8l169.4-169.4c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25l-192 192C240.4 412.9 232.2 416 224 416z"/></svg>
        </h3>

        <div id="projets">
            <a :key="projet.title" v-for="projet in projects" class="card_project" :href="projet.link" target="_blank">
                <img :src="projet.logo" :alt="projet.tilte">
            </a>
        </div>
    </main>
</template>
<!----------Template / Script---------->
<script>
    import { projets } from '../assets/data';
    export default {
        name: 'Projet',
        data() {
            return {
                projects: projets,
            }
        },
    }
</script>
<!----------Script / Style---------->
<style scoped>
    main {
        display: flex;
        flex-direction: column;
        width: 60%;
        min-width: 900px;
        height: auto;
        margin: 0 auto;
		border: 1px solid var(--front);
    }

    h3 {
        display: flex;
        justify-content: center;
        align-items: center;
        overflow: hidden;
        flex-wrap: nowrap;
        width: 100%;
        align-self: center;
        font-size: 1.5em;
        padding: 15px 0;
        border-bottom: 1px solid var(--front);
    }

    h3 svg {
        height: .9em;
        margin: 0 15px;
        fill: var(--front);
    }

    #projets {
        height: auto;
        width: 100%;
        display: flex;
        /* flex-direction: column; */
        align-items: center;
        flex-wrap: wrap;
        flex-shrink: 1;
    }

    .card_project {
        display: flex;
        justify-content: space-around;
        align-items: center;
        height: 120px;
        width: 33%;
        min-width: 299px;
        padding: 10px 30px;
        margin: 10px 0;
    }
    .card_project img {
        object-fit: contain;
        object-position: center;
        height: 75%;
        width: 100%;
        transition-duration: 350ms;
        transition-property: all;
        filter: grayscale(1);
    }

    .card_project:hover img {
        transform: scale(1.1);
        filter: grayscale(0);
    }

    @media screen and (max-width: 940px) {
        main {
            width: 95%;
            min-width: 300px;
        }

        h3 {
            font-size: 1.2em;
        }

        h3 svg {
            height: .7em;
        }

        #projets {
            flex-direction: column;
        }

        .card_project:hover img, .card_project:active img {
            transform: scale(1.1);
            filter: grayscale(0);
        }
    }
</style>