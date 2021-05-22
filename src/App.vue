<template>
    <header class="document__header" />

    <div class="page">
        <div class="page__main">
            <breadcrumbs class="page__breadcrumbs" />

            <search-field placeholder="Поиск по компаниям" />

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
import SearchField from './components/SearchField/SearchField.vue';

export default {
  name: 'App',
  components: {
    Breadcrumbs,
    SearchField,
  },
};
</script>

<style lang="scss">
@import "./components/Page/Page";
</style>
