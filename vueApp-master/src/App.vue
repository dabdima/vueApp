<template>
  <div id="app">
    <ul>
      <li>
        <router-view><img src="./assets/logo.png"></router-view>

      </li>
      <li>
        <router-link to="/admin">admin</router-link>

      </li>
      <li>
        <router-link to="/login">login</router-link>

      </li>
    </ul>


  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style lang="scss">
  body {
    padding:  0px;
    margin: 0px;
  }
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    img {
      width: 50px;
      height: 50px;
    }
    ul {
      display: flex;
      justify-content: space-around;
      li {
        display: flex;
        list-style: none;
        flex-direction: column;
        justify-content: center;
        justify-items: center;
        height: 50px;
        a {
          display: block;
        }
        }
      }

  }
</style>
