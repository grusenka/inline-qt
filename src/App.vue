<template>
    <header class="document__header" />

    <div class="page">
        <div class="page__main">
            <breadcrumbs class="page__breadcrumbs" />

            <main class="main">
                <header class="main-header"></header>

                <div class="main-content"></div>
            </main>

        </div>

        <aside class="page__sidebar"></aside>
    </div>
</template>

<script>
import Breadcrumbs from './components/Breadcrumbs/Breadcrumbs.vue';

export default {
  name: 'App',
  components: {
    Breadcrumbs,
  },
};
</script>

<style lang="scss">
@import "./components/Page/Page";
</style>
