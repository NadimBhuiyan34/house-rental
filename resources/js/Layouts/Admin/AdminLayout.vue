<template>
  <div>
    <Head :title="title" />

    <Banner />

    <div class="flex min-h-screen bg-gray-100">
      <!-- Sidebar -->
      <Sidebar />

      <!-- Main Content -->
      <div class="flex flex-col flex-1">
        <!-- Header -->
        <Header :user="$page.props.auth.user" @logout="logout" />

        <!-- Page Content -->
        <main class="p-6">
          <slot />
        </main>

        <!-- Footer -->
        <Footer />
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import { Head, router } from '@inertiajs/vue3'
import Sidebar from '@/Layouts/Admin/Sidebar.vue'
import Header from '@/Layouts/Admin/Header.vue'
import Footer from '@/Layouts/Admin/Footer.vue'


defineProps({
  title: String,
})

const logout = () => {
  router.post(route('logout'))
}
</script>
