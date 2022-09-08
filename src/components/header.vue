<template>
  <div class="h-screen w-full bg-darkest text-primary">
    <!--Nav-->
    <div class="h-12 container mb-5">
      <ul class="flex justify-end text-right py-5">
        <li class="mx-5 hover:text-secondary"><a href="#home">Home</a></li>
        <li class="mx-5 hover:text-secondary"><a href="#info">Sobre QR</a></li>
        <li class="mx-5 hover:text-secondary"><a href="#generador">QRGenerator</a></li>
        <li class="mx-5 hover:text-secondary"><a href="#contact">Contacto</a></li>
      </ul>
    </div>
    <!--End Nav-->
    <!--Welcome-->
    <div class="container flex flex-wrap justify-around items-center pt-5 my-5" id="home">
      <img class="mt-5 w-80 h-auto contrast-100" src="descarga2.webp" alt="">
      <div class="ml-3 mt-5 py-5">
        <h1 class="text-6xl mb-5">Generador de QR</h1>
        <h3 class="text-3xl mb-5">¡Sumate vos también a la digitalización!</h3>
        <a class="flex mb-5 w-48 items-center justify-center rounded bg-dark hover:bg-secondary hover:text-darkest p-2 border border-secondary my-5" href="#generador">
          Ir al Generador <i class="material-icons items-center ml-3">arrow_downward</i>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style>

</style>