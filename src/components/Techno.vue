<template>
    <div id="techno">
        <img :src="js" alt="javascript"/>
        <img :src="vue" alt="vue"/>
        <img :src="node" alt="node"/>
        <img :src="ex" alt="express"/>
        <img :src="html" alt="html" />
        <img :src="css" alt="css" />
        <img :src="sass" alt="sass" />
    </div>
</template>
<!----------Template / Script---------->
<script>
    export default {
        name: 'Techno',
        data() {
            return {
                js: 'https://img.shields.io/badge/JavaScript-FFFFFF?style=for-the-badge&logo=javascript&logoColor=black',
                vue: 'https://img.shields.io/badge/Vue.js-FFFFFF?style=for-the-badge&logo=vue.js&logoColor=black',
                node: 'https://img.shields.io/badge/Node.js-FFFFFF?style=for-the-badge&logo=node.js&logoColor=black',
                ex: 'https://img.shields.io/badge/Express.js-FFFFFF?style=for-the-badge&logo=Express&logoColor=black',
                html: 'https://img.shields.io/badge/HTML-FFFFFF?style=for-the-badge&logo=html5&logoColor=black',
                css: 'https://img.shields.io/badge/CSS-FFFFFF?style=for-the-badge&logo=css3&logoColor=black',
                sass: 'https://img.shields.io/badge/Sass-FFFFFF?style=for-the-badge&logo=sass&logoColor=black',
            }
        },
    }
</script>
<!----------Script / Style---------->
<style scoped>
    #techno {
        height: 40px;
        width: 900px;
        margin: 0 auto;
        display: flex;
        justify-content: space-around;
        background-color: var(--front);
    }

    img {
        height: 37px;
        width: auto;
    }
</style>