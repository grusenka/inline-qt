<template>
    <table class="table">
        <thead class="table__header">
            <tr class="table__row">
                <th class="table__title">Объявление</th>
                <th class="table__title">Время</th>
                <th class="table__title"><div class="viewings viewings_type_secondary"/></th>
                <th class="table__title">Опубликовал</th>
            </tr>
        </thead>

        <tbody>
            <tr class="table__row" v-for="value in values" :key="value.ID">
                <td class="table__cell">
                    <div class="announcement">
                        <div class="announcement__type">
                            <badge v-if="value.Type === 'sell'" class="badge_type_sell">
                                Продам
                            </badge>

                            <badge v-if="value.Type === 'buy'" class="badge_type_buy">Куплю</badge>
                        </div>
                        <div class="announcement__title">
                            <a class="link" href="#">{{ value.Title }}</a>
                        </div>
                    </div>
                </td>

                <td class="table__cell">{{ value.Date }}</td>

                <td class="table__cell">{{ value.Viewings }}</td>

                <td class="table__cell">
                    <author
                        :name="value.Author.Name"
                        :company="value.Author.Company"
                        :photo="value.Author.Photo"
                    />
                </td>
            </tr>
        </tbody>
    </table>
</template>

<script>
import Badge from '../Badge/Badge.vue';
import Author from '../Author/Author.vue';

export default {
  name: 'last-announcement',
  components: {
    Badge,
    Author,
  },
  data() {
    return {
      values: [
        /* eslint-disable global-require */
        {
          ID: '01',
          Type: 'sell',
          Title: 'Желудки куриные очищенные 60 руб.',
          Date: '5 фев',
          Viewings: 155,
          Author: {
            Name: 'Татьяна Лобач',
            Company: 'Орехово-Зуевский мясокомбинат',
            Photo: require('../../assets/Authors/default.svg'),
          },
        },
        {
          ID: '02',
          Type: 'sell',
          Title: 'ГоленьЦБ(подл) 100р, Желудки кур.очиш 60 р',
          Date: '27 янв',
          Viewings: 185,
          Author: {
            Name: 'Татьяна Лобач',
            Company: 'Орехово-Зуевский мясокомбинат',
            Photo: require('../../assets/Authors/default.svg'),
          },
        },
        {
          ID: '03',
          Type: 'buy',
          Title: 'Курица, Индейка, Говядина, Свинина от МК',
          Date: '21 апр',
          Viewings: 42609,
          Author: {
            Name: 'Татьяна Лобач',
            Company: 'Орехово-Зуевский мясокомбинат',
            Photo: require('../../assets/Authors/default.svg'),
          },
        },
        {
          ID: '04',
          Type: 'buy',
          Title: 'ГоленьЦБ(подл) 100р, Желудки кур.очиш 60 р',
          Date: '27 фев',
          Viewings: 319,
          Author: {
            Name: 'Татьяна Лобач',
            Company: 'Орехово-Зуевский мясокомбинат',
            Photo: require('../../assets/Authors/default.svg'),
          },
        },
        {
          ID: '05',
          Type: 'sell',
          Title: 'Курица, Индейка, Говядина, Свинина от МК',
          Date: '7 фев',
          Viewings: 10072,
          Author: {
            Name: 'Татьяна Лобач',
            Company: 'Орехово-Зуевский мясокомбинат',
            Photo: require('../../assets/Authors/default.svg'),
          },
        },
        {
          ID: '06',
          Type: 'buy',
          Title: 'Фарш куриный ММО люкс 40руб/кг',
          Date: '7 фев',
          Viewings: 300,
          Author: {
            Name: 'Виталий Пчелинцев',
            Company: 'ООО ОКЕАНФИШ',
            Photo: require('../../assets/Authors/01.jpg'),
          },
        },
        {
          ID: '07',
          Type: 'buy',
          Title: 'Голень ЦБ ГОСТ 75 руб/кг',
          Date: '7 фев',
          Viewings: 319,
          Author: {
            Name: 'Виталий Пчелинцев',
            Company: 'ООО ОКЕАНФИШ',
            Photo: require('../../assets/Authors/01.jpg'),
          },
        },
        /* eslint-enable global-require */
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../Table/Table.scss";
@import "../Link/Link.scss";
@import "../Announcement/Announcement.scss";
</style>
