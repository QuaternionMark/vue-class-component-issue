<template>
<p>Value is: {{ booleanProperty }},
    Type is: {{ typeof booleanProperty }}</p>
</template>

<script lang="ts">
import { Options, prop, Vue } from "vue-class-component";

class Props {
    public booleanProperty = prop<boolean>({});
}

export default class HelloWorld extends Vue.with(Props) {
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
    margin: 40px 0 0;
}

ul {
    list-style-type: none;
    padding: 0;
}

li {
    display: inline-block;
    margin: 0 10px;
}

a {
    color: #42B983;
}
</style>
