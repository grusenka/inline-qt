<template>
    <header class="document__header" />

    <div class="page">
        <div class="page__main">
            <breadcrumbs class="page__breadcrumbs" />

            <search-field placeholder="Поиск по компаниям" />

            <action-button
                    class="action-button_icon_previous page__previous"
                    href="#"
            >К каталогу компаний</action-button>

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
import ActionButton from './components/ActionButton/ActionButton.vue';

export default {
  name: 'App',
  components: {
    Breadcrumbs,
    SearchField,
    ActionButton,
  },
};
</script>

<style lang="scss">
@import "./components/Page/Page";
</style>
