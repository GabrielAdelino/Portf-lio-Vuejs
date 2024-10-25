<template>
    <header>
      <nav>
        <ul>
          <li v-for="(link, index) in navLinks" :key="index">
            <a :href="link.href">{{ link.text }}</a>
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
          { text: 'Home', href: '#home' },
          { text: 'About', href: '#about' },
          { text: 'Projects', href: '#projects' },
          { text: 'Contact', href: '#contact' }
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
  list-style-type: none;
  display: flex;
  justify-content: space-between;
  padding: 0;
}

nav ul li a {
  color: white;
  text-decoration: none;
  font-weight: bold;
}

nav ul li a:hover {
  text-decoration: underline;
}
  </style>
  