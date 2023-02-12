<template>
  <nav class="p-6 px-12 flex justify-between items-center font-semibold">
    <header class="font-black">
      <a href="/" target="_self">Badr.ch</a>
    </header>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#about">Work</a></li>
      <li><a href="#services">Process</a></li>
      <li><a href="#">Drop Me A Line</a></li>
    </ul>
    <div>
      <font-awesome-icon class="moon" :icon="['fas', 'moon']" />
    </div>
  </nav>
</template>
<script>
export default {
  name: 'NavBar',
}
</script>
<style lang="postcss" scoped>
ul {
  @apply flex justify-between items-center;
}
ul,
li {
  display: inline;
  @apply mx-2;
}
.moon {
  @apply text-xl;
}
.moon:hover {
  cursor: pointer;
}
</style>
