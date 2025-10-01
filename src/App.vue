<template>
  <h1>CRYPTO</h1>

  <Input />
  <div className="selectors">
    <Selector />
    <Selector />
  </div>
</template>

<script>
import Input from "./components/Input.vue";
import Selector from "./components/Selector.vue";

export default {
  components: { Input, Selector },
};
</script>

<style scoped>
.selectors {
  display: flex;
  justify-content: space-around;
  max-width: 700px;
  width: 100%;
  margin-inline: auto;
}
</style>
