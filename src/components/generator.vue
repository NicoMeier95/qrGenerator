<template>
  <div class="bg-darkest text-primary py-5">
    <h3 class="text-3xl py-3 text-center" id="generador">Generador de QR</h3>
    <div class="container flex flex-wrap items-center py-4 justify-evenly">
      <div class="p-5">
        <img v-bind:src="img">
      </div>
      <form class="ml-5 flex flex-col pt-5">
        <p>Tamaño</p>
        <select v-model="select" class="text-darkest border-0 rounded-sm">
          <option value="300" selected>300x300</option>
        </select>
        <p class="mt-5">Texto para crear tu QR</p>
        <input type="text" class="text-darkest border-0 rounded-sm" v-model="text" placeholder="Ingresa tu texto"/>
        <button class="mt-5 rounded-sm border-2 border-secondary p-1 hover:bg-secondary hover:border-dark hover:text-darkest" type="submit" @click.prevent="genQR" >Submit</button>
        
      </form>
    </div>
  </div>
</template>

<script>
import {ref } from 'vue'

const img = ref('');
const text = ref('');
const select = ref(300)
const gapi = "https://chart.googleapis.com/chart?chf=bg,s,65432100&cht=qr&chs=";


export default {
    name: 'Generator',
    data() {
      return {
        text, select, img, gapi
      }
    },
    methods:{
      genQR(){
        if(text.value !== '' && select.value=="300"){
          img.value = gapi+"300x300"+"&chl="+text.value;
        }else{
          alert('Debes escribir algo!');
        }
        
        this.text = '';

      }
    }
}
</script>

<style>

</style>