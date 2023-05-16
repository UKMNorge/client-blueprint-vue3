<template>
    <div>
        <h1>First Tab</h1>
        <ChildComponent ref="childArrangementer" />
        
        <h2>Fra UKM Komponenter</h2>
        <UKMTable msg='Hello Table test' color="red" />

    </div>
</template>
  
<script setup lang="ts">
    import ChildComponent from '../components/ChildComponent.vue';
    import { ref, onMounted } from 'vue';
    // Import fra UKM Komponenter
    import { UKMTable } from 'ukm-components-vue3';

    const childArrangementer = ref();
    
    onMounted(() => {
        console.log('FirstTab.vue:  onMounted()');
        childArrangementer.value.init();

    });
</script>