<template>
  <div>
    <input ref="inputField" type="text" placeholder="Click the button to focus" />
    <button @click="focusInput">Focus Input</button>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue';

const inputField = ref(null); // DOM 요소에 대한 ref 선언

const focusInput = () => {
  inputField.value.focus(); // ref를 통해 DOM 요소에 접근
};

onMounted(() => {
  console.log(inputField); // 컴포넌트가 마운트된 후, inputField에 접근 가능
  if(inputField.value) {
    inputField.value.focus();
  }
});

// <script setup>에서는 return이 필요 없습니다.
</script>
