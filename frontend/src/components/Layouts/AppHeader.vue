<template>
  <div class="flex border-b pr-5">
    <div id="app-header" class="flex-1"></div>

    <div class="flex items-center space-x-4 justify-center">

      <!-- 🔵 Attendance Button -->
      <button
        @click="openAttendance"
        class="px-3 py-1 rounded bg-purple-600 text-white hover:bg-purple-700 transition"
      >
        Attendance
      </button>

      <!-- Existing Call UI -->
      <CallUI />
    </div>
  </div>
</template>

<script setup>
import CallUI from '@/components/Telephony/CallUI.vue'
import { useRouter } from 'vue-router'

const router = useRouter()

function openAttendance() {
  router.push('/app/attendance-checkin/new-attendance-checkin-oxtvhaxqov')
}
</script>
