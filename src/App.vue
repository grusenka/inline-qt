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
                <main-header />

                <div class="main-content">
                    <section-group>
                        <section-subgroup>
                            <Section header="Последние объявления сотрудников компании">
                            </Section>

                            <Section header="Фото продукции">
                            </Section>
                        </section-subgroup>
                    </section-group>
                </div>
            </main>

        </div>

        <page-sidebar />
    </div>
</template>

<script>
import Breadcrumbs from './components/Breadcrumbs/Breadcrumbs.vue';
import SearchField from './components/SearchField/SearchField.vue';
import ActionButton from './components/ActionButton/ActionButton.vue';
import MainHeader from './components/MainHeader/MainHeader.vue';
import PageSidebar from './components/PageSidebar/PageSidebar.vue';
import SectionGroup from './components/SectionGroup/SectionGroup.vue';
import SectionSubgroup from './components/SectionSubgroup/SectionSubgroup.vue';
import Section from './components/Section/Section.vue';

export default {
  name: 'App',
  components: {
    Breadcrumbs,
    SearchField,
    ActionButton,
    MainHeader,
    PageSidebar,
    SectionGroup,
    SectionSubgroup,
    Section,
  },
};
</script>

<style lang="scss">
@import "./components/Page/Page";
</style>
