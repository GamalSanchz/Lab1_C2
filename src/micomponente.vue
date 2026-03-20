<script setup lang="ts">
import { ref } from 'vue'

interface Material {
  nombre: string
  categoria: string
  cantidad: number
}

const nombre = ref('')
const categoria = ref('')
const cantidad = ref<number | ''>('')
const materiales = ref<Material[]>([])

function agregar() {
  if (!nombre.value || !categoria.value || cantidad.value === '') return
  materiales.value.push({
    nombre: nombre.value,
    categoria: categoria.value,
    cantidad: Number(cantidad.value)
  })
  nombre.value = ''
  categoria.value = ''
  cantidad.value = ''
}
</script>

<template>
  <div class="contenedor">
    <h1>Inventario Escolar</h1>

    <div class="formulario">
      <div class="campo">
        <label>Nombre del material:</label>
        <input v-model="nombre" type="text" placeholder="Ej: Lápiz" />
      </div>
      <div class="campo">
        <label>Categoría:</label>
        <input v-model="categoria" type="text" placeholder="Ej: Escritura" />
      </div>
      <div class="campo">
        <label>Cantidad:</label>
        <input v-model="cantidad" type="number" placeholder="Ej: 10" />
      </div>
      <button @click="agregar">Agregar</button>
    </div>

    <div class="lista">
      <h2>Materiales registrados</h2>
      <p v-if="materiales.length === 0">No hay materiales registrados.</p>
      <ul v-else>
        <li v-for="(m, i) in materiales" :key="i">
          <strong>{{ m.nombre }}</strong> — {{ m.categoria }} — Cantidad: {{ m.cantidad }}
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped></style>