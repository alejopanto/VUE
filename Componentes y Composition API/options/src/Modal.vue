<template>
  <div>
    <button @click="toggle">Modal</button>
    <teleport to="body">
      <div v-show="show" class="modal">
        <h1>Titulo</h1>
        <p>
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quibusdam
          provident adipisci nostrum quaerat explicabo molestias nisi recusandae
          dolor praesentium, aspernatur autem minima iste, officia odit ad
          veritatis totam? Quibusdam, nesciunt?
        </p>
        <button @click="toggle">Cerrar</button>
      </div>
    </teleport>
  </div>
</template>

<script>
export default {
  data() {
    return {
      show: false,
    };
  },
  methods: {
    toggle() {
      this.show = !this.show;
    },
  },
};
</script>
