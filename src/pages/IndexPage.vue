<template>
  <q-page class="flex">
    <div class="q-pa-md row items-start q-gutter-md flex">
      <q-card class="my-card" v-for="card in cards" :key="card">
        <img :src="card.image">
  
        <q-card-section>
          <div class="text-h6">{{card.title}}</div>
          <div class="text-subtitle2">by John Doe</div>
        </q-card-section>
  
        <q-card-section class="q-pt-none">
          {{ card.description }}
        </q-card-section>
      </q-card>

    </div>
  </q-page>
</template>

<script>
export default{
  data(){
    return {
      word:"Quasar",
      cards:[
        {
          image:"https://cdn.quasar.dev/img/mountains.jpg",
          title:"Card1",
          description:"Card1 description"
        },
        {
          image:"https://cdn.quasar.dev/img/mountains.jpg",
          title:"Card2",
          description:"Card2 description"
        },
        {
          image:"https://cdn.quasar.dev/img/mountains.jpg",
          title:"Card3",
          description:"Card3 description"
        },
      ]
    }
  }
}
</script>

<style scoped>
  .my-card{
    width: 100%;
    max-width: 250px
  }
  </style>