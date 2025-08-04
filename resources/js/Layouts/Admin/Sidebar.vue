<template>
  <aside class="w-64 bg-white shadow-lg hidden md:block h-screen fixed">
    <div class="p-6 font-bold text-xl text-blue-600 border-b">
      Admin Panel
    </div>
    <nav class="mt-6">
      <ul>
        <li>
          <Link href="" class="block px-6 py-2 text-gray-700 hover:bg-blue-100 rounded">
            Dashboard
          </Link>
        </li>
        <li>
          <Link href="" class="block px-6 py-2 text-gray-700 hover:bg-blue-100 rounded">
            Properties
          </Link>
        </li>
        <li>
          <Link href="" class="block px-6 py-2 text-gray-700 hover:bg-blue-100 rounded">
            Users
          </Link>
        </li>
        <li>
          <Link href="" class="block px-6 py-2 text-gray-700 hover:bg-blue-100 rounded">
            Bookings
          </Link>
        </li>
      </ul>
    </nav>
  </aside>
</template>

<script setup>
import { Link } from '@inertiajs/vue3'
</script>
