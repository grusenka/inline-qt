<template>
    <a class="action-button" :href="href"><slot /></a>
</template>

<script>
export default {
  name: 'action-button',
};
</script>

<style lang="scss" src="./ActionButton.scss" />
