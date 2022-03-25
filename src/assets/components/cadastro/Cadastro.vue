<template>
  <div class="container">
    <div class="body-form">
      <h1>Cadastro</h1>
      <b-form-input
        v-model="name"
        placeholder="Enter your name"
        class="margin"
      ></b-form-input>
      <b-form-input
        v-model="user"
        placeholder="Enter your username"
      ></b-form-input>
      <b-form-input
        v-model="email"
        placeholder="Enter your e-mail"
      ></b-form-input>
      <label for="password">
        <b-form-input
          type="password"
          v-model="password"
          placeholder="Enter your password"
        ></b-form-input>
      </label>
      <b-button variant="primary">Confirm</b-button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "",
      user: "",
      password: "",
      email: "",
    };
  },
};
</script>

<style>
h1 {
  text-align: center;
  margin-top: 20px;
}

.container {
  display: flex;
  width: 500px;
  height: 100vh;
  align-self: center;
  justify-content: center;
}

.body-form {
  width: 100%;
  display: flex;
  flex-direction: column;
  gap: 10px;
  height: 500px;
  border: 1px solid gray;
  align-self: center;
  padding: 0 15px;
  border-radius: 10px;
}

button {
  margin-top: 40px;
}

.margin {
  margin-top: 50px;
}
</style>