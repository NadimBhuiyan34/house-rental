<template>
  <header class="bg-white shadow px-6 py-4 flex items-center justify-between">
    <h1 class="text-xl font-semibold">Admin Dashboard</h1>

    <div class="flex items-center space-x-4">
      <img
        v-if="user.profile_photo_url"
        :src="user.profile_photo_url"
        alt="Profile"
        class="w-8 h-8 rounded-full object-cover"
      />

      <span class="text-gray-700">{{ user.name }}</span>

      <button
        @click="$emit('logout')"
        class="text-sm text-red-600 hover:underline"
      >
        Logout
      </button>
    </div>
  </header>
</template>

<script setup>
defineProps({
  user: Object,
})
</script>
