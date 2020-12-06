<template>
    
    <div id="carouselExampleCaptions" class="carousel slide" data-ride="carousel">
        <top-menu></top-menu>
        <ol class="carousel-indicators">
            <li data-target="#carouselExampleCaptions" data-slide-to="0" class="active"></li>
            <li data-target="#carouselExampleCaptions" data-slide-to="1" class=""></li>
            <li data-target="#carouselExampleCaptions" data-slide-to="2" class=""></li>
        </ol>
        <div class="carousel-inner">
            <div class="carousel-item active">
                <img src="https://coworkingfy.com/wp-content/uploads/2019/11/trabajo-en-equipo-grupo-figurativo-de-equipo-de-trabajo-1024x612.jpg" alt="Imagen Grupo" width=100%, height=400px>
                <div class="carousel-caption d-none d-md-block">
                    <h5>Trabajo en equipo</h5>
                </div>
            </div>
            <div class="carousel-item">
                <img src="https://www.radiosuperpopayan.com/wp-content/uploads/2020/07/MINTIC.png" alt="Imagen MinTic" width=100%, height=400px>
                <div class="carousel-caption d-none d-md-block">
                    <h5>MinTic</h5>
                </div>
            </div>
            <div class="carousel-item">
                <img src="https://media.utp.edu.co/paginaprincipal/imagenes/banner-nueva-marca-UTP-551A.jpg" alt="Imagen Grupo" width=100%, height=400px>
                <div class="carousel-caption d-none d-md-block">
                    <h5>Trabajo en equipo</h5>
                </div>
            </div>
        </div>
        <a class="carousel-control-prev" href="#carouselExampleCaptions" role="button" data-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="sr-only">Previous</span>
        </a>
        <a class="carousel-control-next" href="#carouselExampleCaptions" role="button" data-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="sr-only">Next</span>
        </a>
    </div>
</template>

<script>
import TopMenu from './TopMenu.vue'
export default {
  components: { TopMenu },
    name : "TopBanner"
}
</script>

<style lang="stylus" scoped>

</style>