<template>
    <dl class="company-information">
        <dt class="company-information__term">Название компании</dt>
        <dd class="company-information__description">
            ООО “Преображенский Мясоперерабатывающий Комбинат”
        </dd>

        <dt class="company-information__term">ОГРН (ОГРНИП)</dt>
        <dd class="company-information__description">1166733069612</dd>

        <dt class="company-information__term">ИНН</dt>
        <dd class="company-information__description">6726022894</dd>

        <dt class="company-information__term">Страна</dt>
        <dd class="company-information__description">Россия</dd>

        <dt class="company-information__term">Регион</dt>
        <dd class="company-information__description">Тверская область</dd>

        <dt class="company-information__term">Описание</dt>
        <dd class="company-information__description">
            Преображенский МПК - современное мясоперерабатывающее предприятие в
            Тверской области.<br/>
            Введен в эксплуатацию в 2013 г. Основу ассортимента составляют порционные и
            мелкокусковые полуфабрикаты из охлажденной свинины. Продукция мясокомбината
            является частью вертикально-интегрированного холдинга КоПИТАНИЯФ.<br/>
            Предприятия холдинга образуют полный цикл производства от выращивания зерна
            и производства комбикормов до производства свежего мяса, что позволяет снизить
            себестоимость и гарантировать безопасность и высокое качество продукции.
        </dd>

        <dt class="company-information__term">Виды деятельности</dt>
        <dd class="company-information__description">
            <ul class="company-information-list">
                <li class="company-information-list__item">Оборудование, упаковка</li>
                <li class="company-information-list__item">Оптовая торговля</li>
                <li class="company-information-list__item">Производитель готовой продукции</li>
                <li class="company-information-list__item">Производитель мясного сырья</li>
                <li class="company-information-list__item">Розничная торговля</li>
            </ul>
        </dd>

        <dt class="company-information__term">Виды продукции</dt>
        <dd class="company-information__description">
            <ul class="company-information-list">
                <li class="company-information-list__item">Свинина</li>
                <li class="company-information-list__item">Замороженное и охлажденное мясо</li>
                <li class="company-information-list__item">Мясные полуфабрикаты</li>
                <li class="company-information-list__item">ПКолбасы, сосиски, деликатесы</li>
            </ul>
        </dd>

        <dt class="company-information__term">Товары и услуги</dt>
        <dd class="company-information__description">
            Мясо замороженное, мясо охлажденное, свинина, субпродукты
        </dd>
    </dl>
</template>

<script>
export default {
  name: 'company-information',
};
</script>

<style lang="scss">
@import './CompanyInformation.scss';
@import '../CompanyInformationList/CompanyInformationList.scss';
</style>
