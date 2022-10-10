<template>
  <svg>
    <use :href="`${sprite}#icon-${icon}`"></use>
  </svg>
</template>
<script setup>
// 使用动态属性时，不能直接写图片路径，需要使用 import 导入
import sprite from "../assets/icons/sprite.svg";

defineProps({
  icon: String,
});
</script>
