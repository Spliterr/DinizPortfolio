<template>
  <div>
    <transition name="fade" appear>
      <div class="modal-overlay" v-if="showModal" @click="$emit('close')"></div>
    </transition>
    <transition name="pop" appear>
      <div class="modal-work">
        <b-carousel-list
          v-model="carouselIdModal"
          :data="items"
          :items-to-show="1"
          :arrow-hover="false"
        >
          <template #item="list">
            <div class="card">
              <div class="card-image">
                <figure class="image is-5by4">
                  <a @click="info(list.index)"
                    ><img :src="list.image" :alt="list.title"
                  /></a>
                </figure>
              </div>
              <div class="card-content">
                <div class="content">
                  <p class="title">{{ list.title }}</p>
                  <p class="subtitle">{{ list.subtitle }}</p>
                </div>
              </div>
            </div>
          </template>
        </b-carousel-list>
      </div>
    </transition>
  </div>
</template>

<script>
export default {
  props: {
    carouselId: Number,
  },
  data() {
    return {
      showModal: true,
      carouselIdModal: this.carouselId,
      items: [
        {
          title: "Lopes - Desenvolvimento de software",
          image: "src/assets/bglopes.png",
          subtitle:
            "Colaborei em uma equipe voltada para serviços free-lances em aplicações web",
        },
        {
          title: "Bocado",
          image: "src/assets/bgbocado.jpg",
          subtitle:
            "Colaborei no desenvolvimento de uma aplicação web para gerenciar os dados do App.",
        },
        {
          title: "Fast Solutions",
          image: "public/img/bgfastsolutions.png",
          subtitle:
            "Realizo o desenvolvimento de uma aplicação web para administrar serviços de print, para clientes e colaboradores.",
        },
      ],
    };
  },
  methods: {
    info(value) {
      this.carouselIdModal = value;
    },
  },
};
</script>

<style>
.modal-work {
  position: absolute;
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  margin: auto;
  text-align: center;
  width: fit-content;
  height: fit-content;
  max-width: 50%;
  border-radius: 1rem;
  box-shadow: 0 5px 5px rgba(0, 0, 0, 0.2);
  z-index: 999;
  transform: none;
}

@media screen and (min-width: 0) and (max-width: 768px) {
  .modal-work {
    max-width: 90% !important;
  }
}

.has-icons-right {
  color: #167df0 !important;
}

.has-icons-left {
  color: #167df0 !important;
}

.carousel-arrow .icon:hover {
  border: 1px solid #167df0 !important;
}

.modal-work h1 {
  margin: 0 0 1rem;
}

.modal-overlay {
  content: "";
  position: absolute;
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 998;
  background: #2c3e50;
  opacity: 0.6;
  cursor: pointer;
}

/* ---------------------------------- */
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.4s linear;
}

.fade-enter,
.fade-leave-to {
  opacity: 0;
}

.pop-enter-active,
.pop-leave-active {
  transition: transform 0.4s cubic-bezier(0.5, 0, 0.5, 1), opacity 0.4s linear;
}

.pop-enter,
.pop-leave-to {
  opacity: 0;
  transform: scale(0.3) translateY(-50%);
}
</style>
