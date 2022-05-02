<template>
  <div class="about">
    <h1 class="title">CONTACT US</h1>
    <h2 class="subtitle">24/7 SUPPORT</h2>
    <section>
      <div class="phone">
        <img src="">
        <h3>Phone
          082 000 0000
        </h3>
      </div>
      <div class="card">
        <span class="text">Name</span><br>
        <input class="input" v-model="message" placeholder=""><br>
        <span class="text">Contact number</span><br>
        <input class="input" v-model="message" placeholder=""><br>
        <span class="text">Email address</span><br>
        <input class="input" v-model="message" placeholder=""><br>
        <span class="text">How can we help you?</span><br>
        <textarea class="input" v-model="message" placeholder=""></textarea>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "about",
  components: {},
};
</script>

<style lang="scss" scoped>
.about {
  .title {
    color: white;
    text-align: left;
    padding-left: 15%;
  }
  .subtitle {
    text-align: left;
    padding-left: 15%;
  }
  .card {
    border: 2px solid white;
    width: 50%;
    display: flex;
    flex-direction: column;
    align-content: right;
    background-color: rgb(43, 42, 42);
    .text {
      color: white;
    }
    .input {
      width: 90%;
    }
  }
}
</style>