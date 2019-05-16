<template>
  <header>
    <nav>
      <div class="logo">
        <router-link to="/">Techno</router-link>
      </div>
      <ul>
        <li>
          <router-link to="/cursos">Cursos</router-link>
        </li>
        <li>
          <router-link to="/contato">Contato</router-link>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script scoped>
export default {
  name: "TheHeader"
};
</script>

<style>
header {
  background: #234;
}

header a {
  color: #fff;
}

a.router-link-exact-active {
  color: #4b8;
}

nav {
  max-width: 800px;
  margin: 0 auto;
  display: flex;
  /* align-content: space-between; */
  justify-content: space-between;
  align-items: center;
  padding: 20px 0;
}

.logo {
  flex: 1;
}

.logo a {
  font-size: 2rem;
  color: #fff;
}

.logo a.router-link-exact-active.router-link-active {
  color: #fff;
}

ul li {
  display: inline-block;
}

li a {
  padding: 0 10px;
  margin-left: 10px;
}
</style>
