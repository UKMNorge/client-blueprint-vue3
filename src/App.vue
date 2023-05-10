<template>
  <!-- apply dark here -->
  <div
    class="max-w-screen min-h-screen bg-base-200 p-2"
    style="font-family: Poppins"
  >
    <div>
        <TheHeader />

        <div class="p-2 grid grid-cols-1 lg:grid-cols-2 flex-wrap gap-4">
            <TheInput />
        </div>

      <TheFooter />
    </div>
  </div>
</template>

<script setup lang="ts">
import TheInput from "./components/TheInput.vue";
import TheHeader from "./components/TheHeader.vue";
import TheFooter from "./components/TheFooter.vue";
import { ref } from "vue";

</script>
