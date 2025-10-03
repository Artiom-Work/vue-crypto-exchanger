<template>
  <input
    min="0"
    type="number"
    @input="changeAmount($event.target.value)"
  /><br />
  <button @click="convert()">Конвертировать</button>
</template>

<script>
export default {
  props: {
    changeAmount: {
      type: Function,
      required: true,
    },
    convert: {
      type: Function,
      required: true,
    },
  },
};
</script>

<style scoped>
input {
  border-radius: 3px;
  border: 0;
  width: clamp(300px, 76vw, 500px);
  position: relative;
  top: -50px;
  outline: none;
  padding: 10px 15px;
  background: #fafafa;
  color: #333;
  font-size: 1.2em;
}

button {
  position: relative;
  top: -20px;
  padding: 15px 20px;
  color: #fff;
  text-transform: uppercase;
  cursor: pointer;
  background: #1a032d;
  border: 0;
  border-radius: 3px;
  transition-duration: 0.3s;
}
button:hover {
  background: #24043e;
}
button:active {
  scale: 0.95;
}
</style>
