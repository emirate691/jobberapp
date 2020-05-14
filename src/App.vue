<template>
  <div>
    <Header />
    <Form />
    <Footer />
  </div>
</template>
<script>
import Header from "./components/Header";
import Footer from "./components/Footer";
import Form from "./components/Form";

export default {
  name: "App",

  components: {
    Header,
    Footer,
    Form,
  },

  data: () => ({
    //
  }),
};
</script>
