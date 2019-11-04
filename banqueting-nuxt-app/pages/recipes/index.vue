<template>
  <section class="recipes">
    <Recipe
      v-for="recipe in recipes"
      :key="recipe.id"
      :thumbnail="recipe.thumbnail"
      :title="recipe.title"
      :id="recipe.id"
      :previewText="recipe.previewText" />
  </section>
</template>

<script>
import Recipe from "@/components/Recipe";

export default {
  components: {
    Recipe
  },
  asyncData() { // Method, "executed" on "server" side in order to fetch all data.
    return new Promise((resolve, reject) => {
      setTimeout(() => {
        resolve({ // Fakes asynchronous request based on promise for 1500 miliseconds
          recipes: [
            {
              id: "1",
              title: "Foto 1",
              previewText: "Descripcion Foto 1",
              thumbnail: "https://scontent-sjc3-1.xx.fbcdn.net/v/t1.0-9/734360_484771634915313_883693630_n.jpg?_nc_cat=104&_nc_oc=AQkjizPHHS20bBxDUqvd5Pcixi_lIWoduY7RcNnXMFFq7EctXPQib5WQ7nJQ1OmgQkc&_nc_ht=scontent-sjc3-1.xx&oh=f382fc3680314fd576617cd6bd66f918&oe=5E60E4C8"
            },
            {
              id: "2",
              title: "Foto 2",
              previewText: "Descripcion Foto 2",
              thumbnail: "https://scontent-sjc3-1.xx.fbcdn.net/v/t1.0-9/69329790_2427333307325793_8614874376166178816_n.jpg?_nc_cat=103&_nc_oc=AQkZ9cMASBt19z7o65gy109y7DPnsqkucDJIHO87eVP0ISJgMfei-4mgVb6H1hhTTnI&_nc_ht=scontent-sjc3-1.xx&oh=a45ec96c02540831fd1e5bf0652ae847&oe=5E516F35"
            }
          ]
        })
       }, 1500)
    })
  }
};
</script>

<style scoped>
.recipes {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-items: center;
}
</style>
