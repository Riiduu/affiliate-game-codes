<template>
  <div class="navbar">
    <div class="main-section">
      <h1>Company name</h1>
      <div class="options">
        <h3>{{ profileName }}</h3>
        <h3>Shop</h3>
      </div>
    </div>

    <div class="end-section">
      <div class="search-bar">
        <input class="search" placeholder="Search"/>
      </div>
      <div class="buttons">
        <button id="login">Log in</button>
        <button id="register">Register</button>
      </div>
    </div>

  </div>
</template>

<script>
export default {
  name: "Navbar-comp",
  components: {

  },
  props: {
    profileName: {
      type: String,
      default: "Anonymous"
    }
  }
}
</script>

<style lang="scss" scoped>
  .navbar {
    height: 100px;
    max-width: 100vw;
    background-color: rgb(14, 22, 40);
    color: white;
    padding: 0 40px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    vertical-align: center;

    .main-section {
      vertical-align: center;
      width: fit-content;
      align-items: center;
      padding: 0 0;
      display: flex;
      flex-direction: row;

      .options {
        display: flex;
        flex-direction: row;
        padding-left: 20px;
      }

      h1 {
        font-size: 1.5rem;
      }

      h3 {
        padding: 0 10px;
      }

      h3, h1 {
        cursor: pointer;
      }
    }

    .end-section {
      display: flex;
      flex-direction: row;
      vertical-align: center;
      position: relative;

      .search-bar {
        align-items: center;
        height: 50px;
        padding-top: 25px;
        padding-right: 20px;

        .search {
          height: 30px;
          border-radius: 30px;
          border: none;
          width: 200px;
          padding: 10px;
        }
      }

      .buttons {
        padding-top: 28px;

        button {
          padding: 10px 30px;
          border-radius: 20px;
          margin: 0 10px;
          color: white;
          font-weight: bold;
          font-size: 1.1rem;
        }

        #login {
          background-color: rgb(88, 173, 67);
        }

        #register {
          background-color: rgb(167, 134, 17);
        }
      }
    }
  }
</style>

