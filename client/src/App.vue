<template>
  <div class="container">
    <Navigation />
    <Header />
    <router-view />
  </div>
</template>

<script>
import Header from './components/Header'
import Navigation from './components/Navigation'

export default {
  name: 'app',
  components: {
    Header,
    Navigation
  }
}
</script>

<style>
  :root {
    --primary-color: #953036;
    --secondary-color: #DE8D00;
  }

  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  body {
    background: var(--primary-color);
    font-family: Arial, Helvetica, sans-serif;
    color: #fff;
    line-height: 1.6;
  }

  a {
    color: #fff;
    text-decoration: none;
  }

  ul {
    list-style: none;
  }

  .body-bg-no-image {
    background: var(--primary-color);
  }

  .body-bg-image {
    background: var(--primary-color) url("./assets/octane.png") no-repeat top center;
  }

  .body-bg-pub-image {
    background: var(--secondary-color);
  }

  .container {
    max-width: 960px;
    margin: 1rem auto;
    overflow: auto;
    padding: 0 rem;
  }

  .form-group {
    margin: 1rem 0;
  }

  .search {
    background: rgba(0, 0, 0, 0.5);
    border: 4px #fff solid;
    margin-top: 1rem;
    padding: 2rem;
  }

  input,
  select,
  textarea {
    display: block;
    width: 100%;
    padding: 0.4rem;
    font-size: 1.2rem;
    border: 1px solid #ccc;
  }

  .bth {
    display: inline-block;
    background: var(--primary-color);
    color: #fff;
    padding: 0.4rem 1.3rem;
    border: none;
    cursor: pointer;
    outline: none;
    margin-top: 1rem;
  }

  @media (max-width: 700px) {
    body {
      background: var(--primary-color);
    }
  }
</style>
