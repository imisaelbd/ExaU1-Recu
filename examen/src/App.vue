<template>
  <div id="app">
    <header>
      <div>
        <b-navbar>
          <b-navbar-nav>
            <b-nav-item href="/home">Home</b-nav-item>
            <b-nav-item href="/form">Form</b-nav-item>
          </b-navbar-nav>
        </b-navbar>
      </div>
    </header>
    <body>
            <div>
              <router-view></router-view>
            </div>
          </body>
   
  </div>
</template>
  
<style scoped>
body {
  margin: 0;
  padding: 0;
  position: relative;
  font-family: Arial, sans-serif;
}

header {
  position: relative;
  z-index: 2;
}

nav {
  background-color: #607274;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}

a.nav-link {
  color: white;
}

.logo {
  font-size: 1.5em;
}

.navbar-links {
  display: flex;
  gap: 20px;
}

.navbar-links a {
  color: white;
  text-decoration: none;
}

.dropdown {
  position: relative;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #333;
  min-width: 160px;
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
  z-index: 1;
}

.dropdown:hover .dropdown-content {
  display: block;
}

.sidebar {
  background-color: #FAEED1;
  color: black;
  height: 100vh;
  width: 250px;
  position: relative;
  transition: margin 0.5s;
}

.sidebar-content {
  padding: 15px;
}

main {
  margin-top: 60px;
  transition: margin 0.5s;
}
</style>