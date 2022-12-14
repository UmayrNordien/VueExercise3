<template>
  <div>
    <AdminTableVue></AdminTableVue>
    <RouterView/>
  </div>
</template>

<script>
import AdminTableVue from '../components/AdminTable.vue';

export default {
  components: {
    AdminTableVue
  }
}
</script>