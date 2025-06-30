<template>
  <div class="min-h-screen bg-gray-50">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8">
      <div class="text-center">
        <h1 class="text-4xl font-bold text-gray-900 mb-4">
          Welcome to {{ appName }}
        </h1>
        <p class="text-xl text-gray-600 mb-8">
          Your central hub for company information and collaboration
        </p>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mt-12">
          <div class="bg-white rounded-lg shadow-md p-6">
            <h3 class="text-lg font-semibold text-gray-900 mb-2">Dashboard</h3>
            <p class="text-gray-600 mb-4">View your personalized dashboard with key metrics and updates.</p>
            <router-link
              to="/dashboard"
              class="inline-flex items-center px-4 py-2 bg-primary-600 text-white rounded-md hover:bg-primary-700 transition-colors"
            >
              Go to Dashboard
            </router-link>
          </div>
          <div class="bg-white rounded-lg shadow-md p-6">
            <h3 class="text-lg font-semibold text-gray-900 mb-2">Employees</h3>
            <p class="text-gray-600 mb-4">Browse employee directory and contact information.</p>
            <router-link
              to="/employees"
              class="inline-flex items-center px-4 py-2 bg-primary-600 text-white rounded-md hover:bg-primary-700 transition-colors"
            >
              View Employees
            </router-link>
          </div>
          <div class="bg-white rounded-lg shadow-md p-6">
            <h3 class="text-lg font-semibold text-gray-900 mb-2">Departments</h3>
            <p class="text-gray-600 mb-4">Explore different departments and their structure.</p>
            <router-link
              to="/departments"
              class="inline-flex items-center px-4 py-2 bg-primary-600 text-white rounded-md hover:bg-primary-700 transition-colors"
            >
              View Departments
            </router-link>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { computed } from 'vue'

const appName = computed(() => import.meta.env.VITE_APP_NAME || 'Company Intranet')
</script>
