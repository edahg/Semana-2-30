<template>
  <div>
    
      <div class="card text-white bg-dark">
        <div class="d-flex justify-content-center p-2">
            <img :src="member.image" alt="Image" height="150px" width = "200px">
        </div>
        <div class="card-body">
          <h4 class="card-title">{{member.nombre}}</h4>
          <h5 class="card-subtitle">{{member.rol}}</h5>
          <p class="card-text"> {{member.descripcion}}</p>
        </div>
        <div class="card-footer">
          <!-- <small class="text-muted">Last updated 3 mins ago</small> -->
          <p> Código: {{member.codigo}} </p>
        </div>
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
