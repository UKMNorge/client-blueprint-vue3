<template>
    <div>
        <h1>First Tab</h1>
        <ChildComponent ref="childArrangementer" />
    </div>
</template>
  
<script setup lang="ts">
    import ChildComponent from '../components/ChildComponent.vue';
    import { ref, onMounted } from 'vue';
    const childArrangementer = ref();
    
    onMounted(() => {
        console.log('FirstTab.vue:  onMounted()');
        childArrangementer.value.init();

    });
</script>