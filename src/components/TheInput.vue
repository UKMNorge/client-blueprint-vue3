<template>
  <div>
    <span>{{ getTextFromObj() }}</span>
    <input placeholder="" />
  </div>
</template>

<script setup lang="ts">
import MyObject from './../objects/myObject'

var myObject = new MyObject();

function getTextFromObj() {
  return myObject.sayHello();
}

</script>

<style>
.scale-enter-active,
.scale-leave-active {
  transition: all 1s ease;
}

.scale-enter-from,
.scale-leave-to {
  opacity: 0;
  transform: scale(0.6);
}
</style>