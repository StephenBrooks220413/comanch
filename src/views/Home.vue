<template>
  <div>
    <div class="bg-image">
      <img
        src="../assets/intro-logo.png"
        class="img-fluid intro"
        alt="Sample"
      />
      <!-- <div class="mask" style="background-color: rgba(0, 0, 0, 0.3)">
        <div class="d-flex justify-content-center align-items-center h-100">
          <h1 class="text-white mb-0">Welcome To Web Development</h1>
        </div>
      </div> -->
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src

@Options({
  components: {
    HelloWorld,
  },
})
export default class Home extends Vue {}
</script>

<style lang="scss" scoped>
@import "../assets/index.css";
.logo {
  width: 150px;
  height: 150px;
}
</style>
