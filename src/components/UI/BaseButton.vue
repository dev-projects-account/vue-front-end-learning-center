<template>
  <button :type="type" :class="mode"><slot></slot></button>
</template>

<script>
export default {
  props: ['type', 'mode']
};
</script>

<style scoped>
button {
  padding: 0.75rem 1.5rem;
  font-family: inherit;
  background-color: #42b883;
  border: 1px solid #3a0061;
  color: white;
  cursor: pointer;
}

button:hover,
button:active {
  background-color: #42b883;
  border-color: #270041;
}

.flat {
  background-color: transparent;
  background-color: #42b883;
  border: none;
}

.flat:hover,
.flat:active {
  background-color: #edd2ff;
}
</style>
