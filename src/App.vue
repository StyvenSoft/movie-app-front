<template>
  <header>
    <router-link to="/">
      <h1><span>App</span>Movies</h1>
    </router-link>
  </header>
  <main>
    <router-view />
  </main>
</template>

<style lang="scss">
$color: #42b883;
$amount: 0.5;

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Fira Sans", sans-serif;

  &::selection {
    background: transparentize($color, $amount);
  }
}

body {
  background-color: #35495e;
}

a {
  text-decoration: none;
}

header {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 10px 16px;
  background-color: #2C3D4E;
  box-shadow: 0 0 6px rgb(0, 0, 0, 0.1);

  h1 {
    color: #fff;
    font-size: 28px;

    span {
      color: $color;
    }
  }
}
</style>
