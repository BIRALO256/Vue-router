<template>
     <div class="max-w-2xl mx-auto p-6 bg-white rounded-lg shadow-lg">
    <h1 class="text-3xl font-bold mb-6 text-gray-800">Available Lectures</h1>
    <div v-for="campus in lectures" :key="campus.id" class="mb-4">
      <router-link
        :to="{ name: 'lectures', params: { id: campus.id } }"
        class="block p-4 bg-gray-100 hover:bg-gray-200 rounded-lg shadow transition"
      >
        <h2 class="text-xl font-semibold text-blue-600">{{ campus.title }}</h2>
      </router-link>
    </div>
  </div>
</template>

<script>
export default {
    data(){
        return{
            lectures :[
                {title: 'Software design preciples',id :1 ,details:'lorem12'},
                {title: 'Embeded systems',id :2 ,details:'lorem12'},
                {title: 'computer leture',id :3 ,details:'lorem12'},
            ]
        }
    }
}
</script>

<style>

</style>