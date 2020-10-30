<template>
  <v-simple-table>
    <template v-slot:default>
      <thead>
        <tr>
          <th class="text-left">Name</th>
          <th class="text-left">ราคา</th>
          <th class="text-left">จำนวน</th>
          <th class="text-left">วันหมดอายุ</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="item in desserts" :key="item.name">
          <td>{{ item.name }}</td>
          <td>{{ item.calories }}</td>
          <td>{{ item.number }}</td>
          <td>{{ item.exp }}</td>
        </tr>
      </tbody>
    </template>
  </v-simple-table>
</template>

<script>
export default {
  data() {
    return {
      desserts: [
        {
          name: 'Frozen Yogurt',
          calories: 159,
          number: 50,
          exp: '10/01/2021',
        },
        {
          name: 'Ice cream sandwich',
          calories: 237,
          number: 50,
          exp: '11/01/2021',
        },
        {
          name: 'Eclair',
          calories: 262,
          number: 50,
          exp: '12/01/2021',
        },
        {
          name: 'Cupcake',
          calories: 305,
          number: 50,
          exp: '13/01/2021',
        },
        {
          name: 'Gingerbread',
          calories: 356,
          number: 50,
          exp: '14/01/2021',
        },
        {
          name: 'Jelly bean',
          calories: 375,
          number: 50,
          exp: '15/01/2021',
        },
        {
          name: 'Lollipop',
          calories: 392,
          number: 50,
          exp: '16/01/2021',
        },
        {
          name: 'Honeycomb',
          calories: 408,
          number: 50,
          exp: '17/01/2021',
        },
        {
          name: 'Donut',
          calories: 452,
          number: 50,
          exp: '18/01/2021',
        },
        {
          name: 'KitKat',
          calories: 518,
          number: 50,
          exp: '19/01/2021',
        },
      ],
    }
  },
}
</script>
