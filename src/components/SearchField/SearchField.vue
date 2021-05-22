<template>
    <div class="search-field">
        <input
            class="search-field__input"
            type="search"
            :placeholder="placeholder"
        />

        <button class="search-field__button">Поиск</button>
    </div>
</template>

<script>
export default {
  name: 'text-field',
  props: ['type', 'placeholder'],
};
</script>

<style lang="scss" src="./SearchField.scss" />
