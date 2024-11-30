<template>
  <div id="app">
    <nav class="navbar navbar-expand-lg navbar-light bg-light mb-4">
      <div class="container">
        <router-link class="navbar-brand" to="/">Gestor de Tareas</router-link>
        <div>
          <router-link class="nav-link" to="/">Home</router-link>
          <router-link class="nav-link" to="/addtask">Agregar Tarea</router-link>
          <router-link class="nav-link" to="/tasklist">Lista de Tareas</router-link>
          <router-link class="nav-link" to="/combined">Vista Combinada</router-link>
        </div>
      </div>
    </nav>
    <router-view />
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
