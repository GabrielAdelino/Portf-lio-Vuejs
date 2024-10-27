<template>
    <header>
      <nav>
        <ul>
          <li v-for="(link, index) in navLinks" :key="index">
            <a :href="link.href">
              <span :class="link.iconStyle">{{ link.icon }}</span>
              {{ link.text }}</a>
            </li>
        </ul>
      </nav>
    </header>
  </template>

  <script>
  export default {
    name: 'AppHeader',
    data() {
      return {
        navLinks: [
          { text: 'Home', href: '#home', icon: "home", iconStyle: "material-icons-outlined"},
          { text: 'About', href: '#about', icon: "account_circle", iconStyle: "material-icons-outlined"},
          { text: 'Projects', href: '#projects', icon: "devices", iconStyle: "material-icons-outlined"},
          { text: 'Contact', href: '#contact', icon: "mail", iconStyle: "material-icons-outlined" }
        ],
      };
  },
  };
  </script>

  <style scoped>

    header {
  background-color: #333;
  color: white;
  margin-top: 0;
  padding: 20px;
}



nav ul {
  font-family: Open Sans, sans serif;
  list-style-type: none;
  display: flex;
  justify-content: space-between;
  padding: 0;
}

nav ul li a {
  color: white;
  text-decoration: none;
  display: inline-block;
  margin-left: 50px;
  font-size: 20px;
  margin-right: 50px; 
  font-weight: bold;
  align-items: center;
  display: flex;
}

.material-icons-outlined{
  display: inline-block;
  text-decoration: none;
  font-size: 30px;
  margin-right: 5px;
  margin-bottom: 5px;
}

/* nav ul li a:hover {
  text-decoration: underline;
} */
  </style>
