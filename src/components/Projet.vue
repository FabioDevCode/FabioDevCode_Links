<template>
    <main>
        <h3>PROJECTS</h3>

        <div id="projets">
            <div :key="projet.title" v-for="projet in projects" class="card_project">
                <img :src="projet.logo" :alt="projet.tilte">
                <h4>{{ projet.title }}</h4>
            </div>
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
        align-self: center;
        font-size: 1.5em;
        padding: 5px 0;
    }

    #projets {
        height: auto;
        width: 100%;
        display: flex;
    }

    .card_project {
        background-color: tomato;
        min-height: 200px;
        min-width: 25%;
    }

</style>