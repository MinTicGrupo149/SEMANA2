<template>
      <div class="card" style="width: 15rem">
            <img :src= "member.imagen" class="img-fluid" alt="..." />
            <div class="card-body">
              <h5 class="card-title">{{member.nombre}}</h5>
              <p class="card-text">{{member.descripcion}}</p>
              <p class="card-text"><span>Rol: </span>{{member.rol}}</p>
              <p class="card-text"><span>Código: </span>{{member.codigo}}</p>
              <a href="https://github.com/juanfpc" class="btn btn-primary">GitHub</a>
          </div>
          </div>
</template>

<script>
export default {
  name: "TeamCard",
  props: ["member"],
};
</script>

<style scoped>
</style>
