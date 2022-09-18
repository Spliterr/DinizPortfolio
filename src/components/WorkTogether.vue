<template>
  <section class="section is-info has-text-centered">
    <div class="container is-narrow">
      <div class="box">
        <div class="columns level">
          <div class="column level-item">
            <h1 class="title">Comece um projeto</h1>
          </div>
          <div class="column level-item">
            <p>Interessado em trabalhar comigo? Deveríamos conversar!</p>
          </div>
          <div class="column level-item">
            <a
              class="button is-info is-outlined is-rounded is-medium"
              href="https://www.linkedin.com/in/felipe-soares-diniz/"
              >Let's do this</a
            >
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.level {
  align-items: center;
  justify-content: space-between;
}

.section {
  padding: 0rem 1.5rem 2rem 1.5rem;
  transform: translatey(75px);
}

@media screen and (min-width: 769px) {
  .level {
    display: flex;
  }
  .level > .level-item:not(.is-narrow) {
    flex-grow: 1;
  }
}

.level-item {
  align-items: center;
  display: flex;
  flex-basis: auto;
  flex-grow: 0;
  flex-shrink: 0;
  justify-content: center;
}

@media screen and (min-width: 769px) {
  .level > .level-item:not(.is-narrow) {
    flex-grow: 1;
  }
}
</style>
