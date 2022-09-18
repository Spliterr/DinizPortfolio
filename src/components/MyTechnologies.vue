<template>
  <section id="my-technologies" class="hero is-info p-5">
    <div class="container is-narrow">
      <div class="box">
        <div class="content">
          <div class="columns is-centered">
            <div class="column card-border-left">
              <div class="card-content">
                <div class="content has-text-centered">
                  <img class="is-centered" src="/img/engineer.png" alt="" />
                  <div class="has-text-dark has-text-centered">
                    <h1 class="eurostile-title is-size-4 is-spaced">
                      Desenvolvimento
                    </h1>
                    <p class="europa-subtitle">
                      Gosto de solucionar problemas, busco ideias e apresento
                      soluções visando a experiência do usuário.
                    </p>
                    <h4 class="europa-subtitle">Minhas skills:</h4>
                    <ul>
                      <li>Interfaces Web Responsivas.</li>
                      <li>Templates, Forms e Rotas.</li>
                      <li>
                        Integrações entre Front-End e Back-End (Api Rest).
                      </li>
                      <li>
                        Correções de problemas e soluções para aprimorar a
                        experiência do usuário.
                      </li>
                      <li>Boa comunicação.</li>
                    </ul>
                  </div>
                </div>
              </div>
            </div>
            <div class="column card-border-center">
              <div class="card-content">
                <div class="content has-text-centered">
                  <img class="is-centered" src="/img/code.png" alt="" />
                  <div class="has-text-dark has-text-centered">
                    <h1 class="eurostile-title is-size-4 is-spaced">
                      Front-end Developer
                    </h1>
                    <p class="europa-subtitle">Frameworks e libs que usei</p>
                    <h4 class="europa-subtitle">Minhas skills:</h4>
                    <ul>
                      <li>Vue.js</li>
                      <li>Vuex</li>
                      <li>Vue-router</li>
                      <li>Javascript</li>
                      <li>Jquery</li>
                      <li>HTML</li>
                      <li>CSS</li>
                      <li>Tailwind</li>
                      <li>Bootstrap</li>
                      <li>Bulma</li>
                      <li>FontAwesome</li>
                      <li>HeroIcons</li>
                    </ul>
                  </div>
                </div>
              </div>
            </div>
            <div class="column card-border-right">
              <div class="card-content">
                <div class="content has-text-centered">
                  <img
                    class="is-centered"
                    src="/img/data-management.png"
                    alt=""
                  />
                  <div class="has-text-dark">
                    <h1 class="eurostile-title is-size-4 is-spaced">
                      Ferramentas:
                    </h1>
                    <p class="europa-subtitle">
                      Ferramentas que utilizei desde quando comecei a trabalhar
                      com desenvolvimento.
                    </p>
                    <h4 class="europa-subtitle">Ferramentas que utilizei:</h4>
                    <ul>
                      <li>Git</li>
                      <li>Bitbucket</li>
                      <li>Github</li>
                      <li>Postman</li>
                      <li>Figma</li>
                      <li>Microsoft Azure</li>
                      <li>Jira</li>
                      <li>FortClient VPN</li>
                    </ul>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
li {
  list-style: none;
  font-family: Europa;
  font-weight: 400;
  margin-left: -30px;
}

.card-border-left {
  background-color: white;
}

.card-border-right {
  background-color: white;
}

.card-border-center {
  border-right: 1px solid #e6ecf8;
  border-left: 1px solid #e6ecf8;
  background-color: white;
}

.mb-7 {
  margin-bottom: 7rem;
}

@media screen and (min-width: 0) and (max-width: 768px) {
  .mb-7 {
    margin-bottom: 5rem;
  }
}
</style>
