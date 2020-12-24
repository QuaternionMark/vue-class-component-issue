<template>
<HelloWorld boolean-property />
<HelloWorld />
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import HelloWorld from "@/components/HelloWorld.vue";

@Options({
    components: {
        HelloWorld
    }
})
export default class App extends Vue {

}
</script>

<style>
/* noinspection CssUnusedSymbol */
#app {
    background-position: top left;
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2C3E50;
}

.main-nav {
    padding: 30px;
    text-align: center;
}

.main-nav a {
    font-weight: bold;
    color: #2C3E50;
}

.main-nav a.router-link-exact-active {
    color: #42B983;
}
</style>
