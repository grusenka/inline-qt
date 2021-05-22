<template>
    <div class="author">
        <div class="author__photo">
            <img class="author__image" :src="photo" alt="Фото автора"/>
        </div>

        <div class="author__information">
            <a class="link author__name" href="#">{{ name }}</a>
            <div class="author__company">{{ company }}</div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'author',
  props: [
    'photo',
    'name',
    'company',
  ],
};
</script>

<style lang="scss" src="./Author.scss"/>
