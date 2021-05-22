<template>
    <header class="main-header">
        <h1 class="main-header__title">Преображениский МПК, ООО</h1>

        <div class="main-header__group">
            <div class="main-header__subgroup">
                <div class="viewings main-header__subgroup-item">578 (+2)</div>

                <action-button
                    class="main-header__subgroup-item
                    action-button_icon_comments action-button_type_secondary"
                >
                    Оставить отзыв
                </action-button>
            </div>

            <Button>Работаете в этой компании?</Button>
        </div>
    </header>
</template>

<script>
import ActionButton from '../ActionButton/ActionButton.vue';
import Button from '../Button/Button.vue';

export default {
  name: 'main-header',
  components: {
    ActionButton,
    Button,
  },
};
</script>

<style lang="scss">
@import "./MainHeader.scss";
@import "../Viewings/Viewings.scss";
</style>
