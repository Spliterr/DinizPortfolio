<template>
  <footer
    class="section is-primary is-small has-text-centered has-background-info"
  >
    <div class="container">
      <figure class="mb-3">
        <a href="#">
          <img
            class="has-background-white-ter img-logo is-centered"
            src="/img/logo-diniz.png"
            alt="Felipe Diniz | Front-end Developer"
        /></a>
      </figure>
      <div class="columns">
        <div class="column">
          <h1 class="title is-size-5-touch eurostile-title has-text-white-ter">
            Vivendo, aprendendo <br />
            e melhorando um dia de cada vez.
          </h1>
        </div>
      </div>
      <div>
        <a
          class="mr-3"
          href="https://www.linkedin.com/in/felipe-soares-diniz/"
          target="_blank"
        >
          <i class="mdi mdi-linkedin mdi-24px p-2 social-icons"></i>
        </a>
        <a
          class="mr-3"
          href="https://www.instagram.com/eu.felipediniz"
          target="_blank"
        >
          <i class="mdi mdi-instagram mdi-24px p-2 social-icons"></i>
        </a>
        <a
          class="mr-3"
          href="mailto:felipesoaresdiniz@gmail.com"
          target="_blank"
        >
          <i class="mdi mdi-email mdi-24px p-2 social-icons"></i>
        </a>
        <a class="mr-3" href="https://github.com/Spliterr" target="_blank">
          <i class="mdi mdi-github mdi-24px p-2 social-icons"></i>
        </a>
      </div>
      <div class="eurostile-title subtitle mt-5 has-text-white-ter">
        Feito por: Felipe Diniz
      </div>
    </div>
  </footer>
</template>

<style scoped>
.img-logo {
  border-radius: 15px;
  width: 80px !important;
  background-color: whitesmoke !important;
}

.social-icons {
  color: #fff !important;
  background: #167df0;
  border-radius: 100%;
  align-items: center;
  display: inline-flex;
  justify-content: center;
  border: 2px solid #ffffff4d;
  width: 2.5rem;
  height: 2.5rem;
}
.social-icons:hover {
  color: #167df0 !important;
  background: #fff;
  border-radius: 100%;
  transform: scale(1.2);
}
</style>
