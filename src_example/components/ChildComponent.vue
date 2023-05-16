<template>
  <div>
    <h1>Child component</h1> 
  </div>
</template>
<script setup lang="ts">
  import MyObject from './../objects/myObject'

  var myObject = new MyObject();

  // Make it accessable through ref
  defineExpose({ init });
  
  function init(){
    console.log('ChildComponent.vue: init()');

    var myObjMethod = myObject.sayHello();
    console.log('From MyObject: ' + myObjMethod);
  }
</script>