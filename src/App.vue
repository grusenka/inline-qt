<template>
    <header class="document__header" />

    <div class="page">
        <div class="page__main">
            <main class="main">
                <header class="main-header"></header>

                <div class="main-content"></div>
            </main>

        </div>

        <aside class="page__sidebar"></aside>
    </div>
</template>

<script>
export default {
  name: 'App',
};
</script>

<style lang="scss">
@import "./components/Page/Page";
</style>
