<template>
  <div class="app__header">
    <NLink to="/" class="header__logo">
      <img src="../assets/logo.png" class="header__icon" alt="logo"/>
      <h1>Rbnb</h1>
    </NLink>
    <div class="header__links">
      <NLink to="/login">
        Login
      </NLink>
      <NLink to="/register">
        Register
      </NLink>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue';

export default {
  components: {
    Logo,
  }
}
</script>
<style>
  .app__header {
    display: flex;
    justify-content: space-between;
    border-bottom: 1px solid #e4e4e4;
    box-shadow: 0 1px 5px rgba(0,0,0,.1);
    padding: 16px 12px 16px 24px;
  }

  .app__header .header__logo {
    display: flex;
    align-items: center;
    text-decoration: none;
  }

  .app__header h1 {
    text-decoration: none;
    color: #4fc08d;
    margin: 0 10px;
  }

  .header__icon {
    height: 34px;
  }

  .header__links {
    display: flex;
    align-items: center;
  }

  .header__links a {
    text-decoration: none;
    line-height: 1;
    color: inherit;
    font-size: 13px;
    letter-spacing: .5px;
    cursor: pointer;
    padding: 8px 10px;
    opacity: 0.8;
  }

  .header__links a:hover {
    border-bottom: 2px solid #484848;
    padding-bottom: 6px;
    opacity: 1;
  }

</style>