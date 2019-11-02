<template>
  <section class="single-recipe">
    <h1>{{ recipe.title }}</h1>
    <div>
      <img class=recipe-image" :src="recipe.thumbnail" :alt="recipe.title">
    </div>
    <p>{{ recipe.descriptionText }}</p>
  </section>
</template>

<script>
export default {
  asyncData(context) {
    return new Promise((resolve, reject) => {
      setTimeout(() => {
        resolve({
          recipe: [
            {
              id: "1",
              title: "Foto 1",
              previewText: "Descripcion Foto 1",
              descriptionText: "This is description foto",
              thumbnail:"https://scontent-sjc3-1.xx.fbcdn.net/v/t1.0-9/734360_484771634915313_883693630_n.jpg?_nc_cat=104&_nc_oc=AQkjizPHHS20bBxDUqvd5Pcixi_lIWoduY7RcNnXMFFq7EctXPQib5WQ7nJQ1OmgQkc&_nc_ht=scontent-sjc3-1.xx&oh=f382fc3680314fd576617cd6bd66f918&oe=5E60E4C8"
            },
            {
              id: "2",
              title: "Foto 2",
              previewText: "Descripcion Foto 2",
              descriptionText: "This is description foto",
              thumbnail:"https://scontent-sjc3-1.xx.fbcdn.net/v/t1.0-9/69329790_2427333307325793_8614874376166178816_n.jpg?_nc_cat=103&_nc_oc=AQkZ9cMASBt19z7o65gy109y7DPnsqkucDJIHO87eVP0ISJgMfei-4mgVb6H1hhTTnI&_nc_ht=scontent-sjc3-1.xx&oh=a45ec96c02540831fd1e5bf0652ae847&oe=5E516F35"
            }
          ].find(el => el.id === context.params.id)
        })
       }, 1500)
    })
  }
}
</script>

<style scoped>
.single-recipe {
  display: flex;
  flex-flow: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding: 3px;
}

.recipe-image {
  width: 100%;
}
</style>
