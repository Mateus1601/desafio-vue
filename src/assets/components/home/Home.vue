<template>
  <div class="page-content">
    <div class="container">
      <h1>Game Store</h1>
      <div class="user-info">
        <p>
          User Name
          <b-dropdown id="dropdown-1" text="" class="m-md-2">
            <b-dropdown-item>Edit Info</b-dropdown-item>
            <b-dropdown-item>Logout</b-dropdown-item>
          </b-dropdown>
        </p>
      </div>
    </div>
    <div>
      <div class="table">
        <b-table striped hover :items="items" :fields="fields"></b-table>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      fields: ["Game", "User", "timePost"],
      items: [
        {
          game: "",
          user: "",
          time: "",
        },
      ],
    };
  },
};
</script>

<style>
.page-content {
  width: 100%;
}

.container {
  display: flex;
  width: 100%;
  justify-content: space-between;
}

.table {
  max-width: 80%;
  margin-left: 150px;
}
</style>