<script setup>
import Logo from "./components/Logo.vue";
import DataInput from "./components/DataInput.vue";
import Or from "./components/Or.vue";
import FB from "./components/FB.vue";
</script>

<template>
  <div class="block">
    <div class="column">
      <Logo />
      <DataInput />
      <Or />
      <FB />
    </div>
  </div>
</template>

<script>

export default {

}
</script>

<style scoped>

.block {
  color: rgb(0,0,0);
  display: flex;
  flex-direction: column;
  justify-content: center;
  max-width: 350px;
  width: 100%;
  margin: auto;
}

.column { /*ab21*/
  align-items: center;
  background-color: rgb(255,255,255);
  border: 1px solid rgb(219,219,219);
  display: flex;
  flex-direction: column;
  font-size: 100%;
  margin-top: 80px;
}
</style>