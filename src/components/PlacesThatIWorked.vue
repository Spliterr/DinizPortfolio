<template>
  <section id="companies" class="skills has-background-white-ter p-5">
    <div class="container">
      <h1 class="eurostile-title title has-text-centered">
        Lugares que trabalhei:
      </h1>

      <div>
        <div class="columns is-variable is-8 mt-3">
          <div class="column image-hover">
            <figure class="image">
              <img
                class="img-job"
                src="../assets/bglopes.png"
                alt="Placeholder image"
              />
              <b-button
                class="btn"
                id="show-modal"
                @click="modalInfo(0)"
                type="is-info is-light"
                >Detalhes</b-button
              >
            </figure>
          </div>
          <div class="column image-hover">
            <figure class="image">
              <img
                class="img-job"
                src="../assets/bg-bocado-small.webp"
                alt="Placeholder image"
              />
              <b-button
                class="btn"
                id="show-modal"
                @click="modalInfo(1)"
                type="is-info is-light"
                >Detalhes</b-button
              >
            </figure>
          </div>
          <div class="column image-hover">
            <figure class="image">
              <img
                class="img-job"
                src="../assets/bgfastsolutions.png"
                alt="Placeholder image"
              />
              <b-button
                class="btn"
                id="show-modal"
                @click="modalInfo(2)"
                type="is-info is-light"
                >Detalhes</b-button
              >
            </figure>
          </div>
        </div>
      </div>
    </div>

    <Modal v-if="showModal" :carouselId="id" @close="showModal = false"></Modal>
  </section>
</template>

<script>
import Modal from "../components/ModalWorkPlaces.vue";

export default {
  name: "PlacesThatIWorked",

  components: {
    Modal,
  },
  data() {
    return {
      showModal: false,
      id: 0,
    };
  },
  methods: {
    modalInfo(idx) {
      this.showModal = true;
      this.id = idx;
    },
  },
};
</script>

<style scoped>
.skills {
  padding: 0;
}

.img-job {
  border-radius: 12px;
  max-height: 200px;
  min-height: 200px;
}

.image-hover figure img {
  -webkit-filter: blur(0);
  filter: blur(0);
  -webkit-transition: 0.3s ease-in-out;
  transition: 0.3s ease-in-out;
  -webkit-transform: scale(1);
  transform: scale(1);
}
.image-hover figure:hover img {
  -webkit-filter: blur(3px);
  filter: blur(3px);
  -webkit-transform: scale(1.1);
  transform: scale(1.1);
  color: #167df0;
}

/* Style the button and place it in the middle of the container/image */
.btn {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  visibility: hidden;
}

img:hover + .btn,
.btn:hover {
  visibility: visible;
  -webkit-transition: 0.4s ease-in;
  transition: 0.4s ease-in;
}
</style>
