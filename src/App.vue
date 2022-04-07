<template>
  <div id="app">
    <header>
      <Header />
    </header>
    <main>
      <Main />
    </main>
    <footer>
      <Footer />
    </footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";
export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Coming+Soon&family=Lato:wght@700&family=Lexend:wght@100;200;300;400;500;600;700;800;900&family=M+PLUS+Rounded+1c:wght@100;300;400;500;700;800;900&family=Montserrat:wght@600;700&family=Patrick+Hand&family=Roboto:wght@300&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Coming+Soon&family=Lato:wght@700&family=M+PLUS+Rounded+1c:wght@100;300;400;500;700;800;900&family=Montserrat:wght@600;700&family=Roboto:wght@300&display=swap");
@import "./components/style/main-style.scss";
* {
  font-family: "M PLUS Rounded 1c", sans-serif;
}
</style>
