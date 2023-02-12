<template>
  <div class="smooth-scroll min-h-screen">
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Raleway&display=swap"
      rel="stylesheet"
    />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Cabin:wght@500&display=swap"
      rel="stylesheet"
    />
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css"
    />
    <NavBar />
    <WelcomeSection />
    <AboutMe />
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>

<style lang="postcss">
* {
  font-family: 'Raleway', sans-serif;
  font-size: 17px;
}
body {
  background-color: #ecf9ff;
  margin: 0;
}

a {
  position: relative;
  color: #000;
  text-decoration: none;
}

a::before {
  content: '';
  position: absolute;
  display: block;
  width: 100%;
  height: 2px;
  bottom: 0;
  left: 0;
  background-color: #000;
  transform: scaleX(0);
  transform-origin: top left;
  transition: transform 0.3s ease;
}

a:hover::before {
  transform: scaleX(1);
}
</style>
