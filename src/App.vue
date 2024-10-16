<script setup>
import Tarjeta from './components/Tarjeta.vue'
import Producto from './components/Producto.vue'
import Avatar from './components/Avatar.vue'
import Usuario from './components/Usuario.vue'
import EstadoPedido from './components/EstadoPedido.vue'
export default {
  name:`App`,
  components: {
    Tarjeta,
    Producto,
    Avatar,
    Usuario,
    EstadoPedido
  },
  data() {
    return {
      nombre: 'Lorena',
      apellido: 'Alarcon',
      edad: 41,
      precio: 10.99,
      url: 'https://picsum.photos/200/300',
      tamaño: 100,
      usuario: {
        nombre: 'Lorena',
        apellido: 'Gonzalez',

</script>

<template>
 <div class="container">
  <Tarjeta :nombre="Instrumento de practica 1" :descripcion="`Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmodtempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodoconsequat. Duis aute irure dolor in reprehenderit in voluptate velit essecillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat nonproident, sunt in culpa qui officia deserunt mollit anim id est laborum.`" />
  <Producto :nombre="Instrumento de practica 2" :precio="precio" />
  <Avatar :url="url" :tamaño="tamaño" />
  <Usuario :usuario="usuario" />
  <EstadoPedido :estado="estado" />
 </div>
</template>

<style scoped>

</style>
