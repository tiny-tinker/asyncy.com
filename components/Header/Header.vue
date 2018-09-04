<template>
  <a-nav class="asyncy-navbar" logo="/img/logo.svg" :isBeta="true" effect="light" expand type="secondary">
    <div class="row" slot="content-header" slot-scope="{closeMenu}">
      <div class="col-6 collapse-brand">
        <a href="./index.html">
          <img src="img/brand/blue.png">
        </a>
      </div>
      <div class="col-6 collapse-close">
        <a-close-button @click="closeMenu">
        </a-close-button>
      </div>
    </div>
    <div class="row" slot="content-header" slot-scope="{closeMenu}">
      <div class="col-6 collapse-brand">
        <a href="./index.html">
            Asyncy
        </a>
      </div>
      <div class="col-6 collapse-close">
        <a-close-button target="nav-inner-primary" v-on:click="closeMenu">

        </a-close-button>
      </div>
    </div>

    <ul class="navbar-nav ml-lg-auto">
      <li class="nav-item">
        <a class="nav-link nav-link-icon" href="#">
          Platform
        </a>
      </li>
      <li class="nav-item">
        <a class="nav-link nav-link-icon" href="#">
          Documentation
        </a>
      </li>
      <li class="nav-item">
        <a class="nav-link nav-link-icon" href="#">
          About
        </a>
      </li>
      <li class="nav-item">
        <a class="nav-link nav-link-icon" href="#">
          Events
        </a>
      </li>
      <li class="nav-item">
        <a class="nav-link nav-link-icon" href="#">
          Contact
        </a>
      </li>
      <li class="nav-item">
        <a class="nav-link nav-link-icon hide-decoration" href="#" style="color:var(--pink)">
          We are Hiring!
        </a>
      </li>
    </ul>
  </a-nav>
</template>

<script>

</script>

<style scoped>
  .asyncy-navbar {
    padding: 35px 0;
  }
</style>
