<template>
  <div class="container">
    <div class="body-form">
      <h1>Login</h1>
      <b-form-input v-model="text" placeholder="Enter your user"></b-form-input>
      <label for="password">
        <b-form-input
          type="password"
          v-model="password"
          placeholder="Enter your password"
        ></b-form-input>
      </label>
      <b-button variant="primary">Sign up</b-button>
      <div class="links">
        <p>Don't have an account?</p>
        <a href="#" style="cursor: pointer">Sign up here</a>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      text: "",
      password: "",
    };
  },
};
</script>
    
<script>
export default {
  data() {
    return {};
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;1,100;1,200;1,300;1,400;1,500;1,600&family=Roboto:ital,wght@0,100;0,300;0,400;1,100;1,300;1,400&display=swap");

.container {
  width: 100%;
  display: flex;
  justify-content: center;
  height: 100vh;
}

.body-form {
  display: flex;
  flex-direction: column;
  align-self: center;
  width: 450px;
  gap: 10px;
  height: 80%;
  border: 1px solid gray;
  padding-right: 20px;
  padding-left: 20px;
  border-radius: 15px;
}

.body-form h1 {
  display: flex;
  justify-content: center;
  font-family: "Roboto", "sans-serif";
  font-weight: bold;
  margin-top: 20px;
  margin-bottom: 100px;
  padding-top: 20px;
}

a {
  align-self: end;
}

.links {
  display: flex;
  gap: 5px;
  margin-top: 40px;
}

.links p {
  margin: 0;
}

button {
  margin-top: 20px;
}
</style>