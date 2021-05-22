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
                                <last-announcement />
                            </Section>

                            <Section header="Фото продукции">
                                <product-list />
                            </Section>
                        </section-subgroup>

                        <company class="section-subgroup">
                            <template v-slot:header>
                                <img src="./assets/ComponyHeader.png" alt="Преображенский МПК"/>
                            </template>

                            <company-information/>
                        </company>
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
import LastAnnouncement from './components/LastAnnouncement/LastAnnouncement.vue';
import Company from './components/Company/Company.vue';
import CompanyInformation from './components/CompanyInformation/CompanyInformation.vue';
import ProductList from './components/ProductList/ProductList.vue';

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
    LastAnnouncement,
    Company,
    CompanyInformation,
    ProductList,
  },
};
</script>

<style lang="scss">
@import "./components/Page/Page";
</style>
