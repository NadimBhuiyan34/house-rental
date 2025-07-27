<template>
  <AdminLayout>
    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
      <div class="bg-white rounded-2xl shadow p-6">
        <h2 class="text-lg font-semibold mb-2">Total Users</h2>
        <p class="text-3xl font-bold text-blue-600">123</p>
      </div>

      <div class="bg-white rounded-2xl shadow p-6">
        <h2 class="text-lg font-semibold mb-2">Total Properties</h2>
        <p class="text-3xl font-bold text-green-600">45</p>
      </div>

      <div class="bg-white rounded-2xl shadow p-6">
        <h2 class="text-lg font-semibold mb-2">Bookings</h2>
        <p class="text-3xl font-bold text-red-600">89</p>
      </div>
    </div>
  </AdminLayout>
</template>

<script setup>
import AdminLayout from '@/Layouts/Admin/AdminLayout.vue'
</script>
