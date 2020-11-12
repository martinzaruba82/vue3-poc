<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld
      msg="Hello world component with standard syntax typescript component"
    />
    <HelloWorldClassSyntax
      msg="Hello world component with class syntax typescript"
    />
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import HelloWorld from "@/components/HelloWorld.vue";
import HelloWorldClassSyntax from "@/components/HelloWorldClassSyntax.vue";

@Options({
  components: {
    HelloWorld,
    HelloWorldClassSyntax
  }
})
export default class Home extends Vue {}
</script>
