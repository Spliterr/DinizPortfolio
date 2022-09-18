<template class="has-background-white-ter">
  <b-navbar class="container">
    <template #brand>
      <b-navbar-item>
        <img src="../assets/logotipofelipeFundoTransparente.png" alt="" />
      </b-navbar-item>
    </template>

    <template #end>
      <b-navbar-item href="#who-iam" class="has-text-info">
        <span>Sobre mim</span>
      </b-navbar-item>
      <b-navbar-item href="#my-technologies" class="has-text-info">
        <span>Tecnologias</span>
      </b-navbar-item>
      <b-navbar-item href="#companies" class="has-text-info">
        <span>Empresas</span>
      </b-navbar-item>
    </template>
  </b-navbar>
</template>

<style scoped>
@media screen and (min-width: 1024px) {
  .navbar-item,
  .navbar-link {
    border-radius: 15px;
    margin: 5px 0px 5px 0px;
    height: 50px !important;
    align-items: center !important;
    display: flex;
  }

  .navbar-item .navbar-link,
  span {
    border: 1px solid #167df0;
    border-radius: 15px;
    padding: 0px 8px 0px 8px;
    height: 50px !important;
    align-items: center !important;
    display: flex;
  }

  a.navbar-item:focus,
  a.navbar-item:focus-within,
  a.navbar-item:hover,
  a.navbar-item.is-active,
  .navbar-link:focus,
  .navbar-link:focus-within,
  .navbar-link:hover,
  .navbar-link.is-active {
    background-color: transparent !important;
  }

  .navbar-item .navbar-link,
  span:hover {
    background-color: #167df0;
    color: #fff !important;
    border-radius: 15px;
    height: 50px !important;
    align-items: center !important;
    display: flex;
  }
}

.navbar-item img {
  max-height: 50px !important;
  scale: 2;
}

@media screen and (min-width: 0) and (max-width: 768px) {
  .navbar-item img {
    scale: 2;
    max-height: 40px !important;
  }
}
</style>
