<template>
    <div>
        <!-- Tabs -->
        <FirstTab />
    </div>
</template>

<script setup lang="ts">
import FirstTab from './tabs/FirstTab.vue';
import { SPAInteraction } from 'ukm-spa/SPAInteraction';
import { Director } from 'ukm-spa/Director';
import { onMounted } from 'vue'


    var name: "World";
    var activeTab : 'arrangementer'

    onMounted(() => {
        console.log('App.vue:  onMounted()');
        console.log(SPAInteraction);
        console.log(Director);        
    });
</script>
