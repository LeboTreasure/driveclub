<template>
  <div class="contact">
    <h1 class="title">CONTACT US</h1>
    <h2 class="subtitle">24/7 SUPPORT</h2>
    <section>
      <div class="card">
        <div class="phone">
          <img src="" />
          <h3>
            Phone <br />
            082 000 0000
          </h3>
        </div>

        <div class="email">
          <img src="" />
          <h3>
            Email <br />
            email@example.com
          </h3>
        </div>

        <div class="location">
          <img src="" />
          <h3>
            Location <br />
            42 Business Rd
          </h3>
        </div>

        <div class="card">
          <h2 class="heading">HOW CAN WE HELP?</h2>
          <b-form @submit="onSubmit" @reset="onReset" v-if="show">
            <b-form-group id="input-group-1" label="Name" label-for="input-1">
              <b-form-input
                id="input-1"
                v-model="form.name"
                required
              ></b-form-input>
            </b-form-group>

            <b-form-group
              id="input-group-2"
              label="Contact number"
              label-for="input-2"
            >
              <b-form-input
                id="input-2"
                v-model="form.name"
                required
              ></b-form-input>
            </b-form-group>

            <b-form-group id="input-group-3" label="Email" label-for="input-3">
              <b-form-input
                id="input-3"
                v-model="form.email"
                type="email"
                required
              ></b-form-input>
            </b-form-group>

            <b-form-group
              id="input 4"
              label="How can we help you?"
              label-for="input 4"
            >
              <b-form-textarea
                id="textarea"
                v-model="text"
                rows="3"
                max-rows="6"
              ></b-form-textarea>
            </b-form-group>

            <b-button class="submit" type="submit" variant="primary">Submit</b-button>

          </b-form>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "contact",
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
    .heading {
      color: white;
    }
    .submit {
      background-color: maroon;
      border: 2px solid red;
    }
  }
}
</style>
