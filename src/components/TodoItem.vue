<template>
    <div class="card mb-2">
    <div class="card-body">
      <h5
        :class="{
          'text-decoration-line-through': completed,
        }"
      >
        {{ title }}
      </h5>
      <p>{{ completed ? 'Completada' : 'Pendiente' }}</p>
      <button class="btn btn-primary btn-sm" @click="$emit('toggle-completion')">
        {{ completed ? 'Marcar como Pendiente' : 'Marcar como Completada' }}
      </button>
      <button class="btn btn-danger btn-sm" @click="$emit('delTodo')">Eliminar</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TodoItem',
  props: {
    title: String,
    completed: Boolean,
  },
};
</script>

<style scoped>
/* Puedes agregar tus propios estilos aquí */
/* Por ejemplo, cambia el color de fondo de las tareas completadas */

</style>