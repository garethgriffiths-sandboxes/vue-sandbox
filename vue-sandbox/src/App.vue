<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
html,
body {
    position: relative;
    width: 100%;
    height: 100%;
}

body {
    font-size: 16px;
    line-height: 24px;
    color: #333;
    margin: 0;
    padding: 8px;
    box-sizing: border-box;
    font-family: "Poppins", Roboto, Oxygen-Sans, Ubuntu, Cantarell, "Helvetica Neue", sans-serif;
}

h4 {
    font-size: 18px;
    line-height: 26px;
}

a {
    color: #4e8b27;
    text-decoration: none;
}

a:hover {
    text-decoration: underline;
}

label {
    display: block;
}

input,
button,
select,
textarea {
    font-family: inherit;
    font-size: inherit;
    -webkit-padding: 0.4em 0;
    padding: 0.4em;
    margin: 0 0 0.5em 0;
    box-sizing: border-box;
    border: 1px solid #ccc;
    border-radius: 2px;
}

input:disabled {
    color: #ccc;
}

button {
    color: #333;
    background-color: #f4f4f4;
    outline: none;
}

button:disabled {
    color: #999;
}

button:not(:disabled):active {
    background-color: #ddd;
}

button:focus {
    border-color: #666;
}

#nav {
  display: none;
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>