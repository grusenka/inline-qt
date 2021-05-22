<template>
<ul class="product-list">
    <li v-for="value in values" :key="value.ID" class="product-list__item">
        <img :src="value.Image" class="product-list__image" alt="Фото продукции"/>
    </li>
</ul>
</template>

<script>
export default {
  name: 'product-list',
  data() {
    return {
      values: [
        /* eslint-disable global-require */
        { ID: '01', Image: require('../../assets/Products/01.jpg') },
        { ID: '02', Image: require('../../assets/Products/02.jpg') },
        { ID: '03', Image: require('../../assets/Products/01.jpg') },
        { ID: '04', Image: require('../../assets/Products/03.jpg') },
        { ID: '05', Image: require('../../assets/Products/04.jpg') },
        { ID: '06', Image: require('../../assets/Products/02.jpg') },
        { ID: '07', Image: require('../../assets/Products/02.jpg') },
        { ID: '08', Image: require('../../assets/Products/01.jpg') },
        { ID: '09', Image: require('../../assets/Products/03.jpg') },
        { ID: '10', Image: require('../../assets/Products/04.jpg') },
        /* eslint-enable global-require */
      ],
    };
  },
};
</script>

<style lang="scss" src="./ProductList.scss"/>
