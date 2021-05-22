<template>
    <aside class="page__sidebar">
        <ul class="banner-list">
            <li class="banner-list__item">
                <div class="banner">Реклама</div>
            </li>

            <li class="banner-list__item">
                <div class="banner">Реклама</div>
            </li>
        </ul>
    </aside>
</template>

<script>
export default {
  name: 'page-sidebar',
};
</script>

<style lang="scss">
@import "./PageSidebar.scss";
@import "../BannerList/BannerList.scss";
@import "../Banner/Banner.scss";
</style>
