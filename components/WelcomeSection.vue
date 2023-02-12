<template>
  <div>
    <section id="home" class="px-12 max-h-full max-w-full">
      <div class="w-full h-full flex flex-col justify-end items-start">
        <div class="flex justify-around flex-row items-end space-x-32">
          <div class="animate__animated animate__fadeIn -space-y-24">
            <h1>Web</h1>
            <h1>Developer</h1>
          </div>

          <div class="h-full flex items-end pb-20 w-full">
            <span class="font-bold">
              Specialized in Web Design, Back End, and Front End Development.
            </span>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'WelcomeSection',
}
</script>
<style lang="postcss" scoped>
h1 {
  font-size: 190px;
  font-family: 'Cabin', sans-serif;
  font-weight: 400;
  margin: 0;
}

section {
  height: 95vh;
}
</style>
