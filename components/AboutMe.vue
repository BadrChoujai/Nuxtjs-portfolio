<template>
  <div class="max-h-full max-w-full">
    <section
      id="about"
      class="mt-8 px-12 h-full w-full flex justify-between items-start"
    >
      <div class="w-7/12 flex justify-start flex-col items-start space-y-8">
        <p class="font-extrabold text-3xl break-words">
          I'm helping startups and business owners to make a visual statement
          through spotless Web Design and Development so they can increase brand
          awareness and sell more.
        </p>

        <button class="resume" role="button">
          Drop Me A Line
          <font-awesome-icon class="env" :icon="['fas', 'envelope']" />
        </button>
      </div>

      <div class="w-1/5 flex justify-start flex-col items-start">
        <span class="font-thin text-sm text-gray-500">Let's get connected</span>
        <div class="thin-line"></div>
        <ul>
          <li><a href="#">Github</a></li>
          <li><a href="#">LinkedIn</a></li>
          <li><a href="#">Instagram</a></li>
        </ul>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'AboutMe',
}
</script>
<style lang="postcss" scoped>
/* CSS */
.resume {
  @apply px-12;
  align-items: center;
  background-color: #ecf9ff;
  border: 2px solid #111;
  border-radius: 25px;
  box-sizing: border-box;
  color: #111;
  cursor: pointer;
  display: flex;
  font-family: Inter, sans-serif;
  font-size: 16px;
  height: 48px;
  justify-content: center;
  line-height: 24px;
  max-width: 100%;
  padding: 0 20px;
  position: relative;
  text-align: center;
  text-decoration: none;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
}

.resume:after {
  background-color: #111;
  border-radius: 25px;
  content: '';
  display: block;
  height: 48px;
  left: 0;
  width: 100%;
  position: absolute;
  top: -2px;
  transform: translate(8px, 8px);
  transition: transform 0.2s ease-out;
  z-index: -1;
}

.resume:hover:after {
  transform: translate(0, 0);
}

.resume:active {
  background-color: #ffdeda;
  outline: 0;
}

.resume:hover {
  outline: 0;
}

@media (min-width: 768px) {
  .resume {
    padding: 0 40px;
  }
}
.env {
  margin-left: 10px;
  width: 20px;
  height: 20px;
}

.thin-line {
  height: 0.3px;
  @apply bg-gray-400 w-full my-4;
}

ul,
li {
  @apply my-2 mt-0;
}
section {
  height: 95vh;
}
</style>
