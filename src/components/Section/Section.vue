<template>
    <section class="section">
        <h2 class="section__header">{{ header }}</h2>

        <div class="section__content"><slot /></div>
    </section>
</template>

<script>
export default {
  name: 'section',
  props: ['header'],
};
</script>

<style lang="scss" src="./Section.scss" />
