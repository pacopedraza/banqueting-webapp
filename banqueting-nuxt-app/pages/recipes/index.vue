<template>
  <section class="recipes">
    <Recipe
      thumbnail="https://scontent-sjc3-1.xx.fbcdn.net/v/t1.0-9/734360_484771634915313_883693630_n.jpg?_nc_cat=104&_nc_oc=AQkjizPHHS20bBxDUqvd5Pcixi_lIWoduY7RcNnXMFFq7EctXPQib5WQ7nJQ1OmgQkc&_nc_ht=scontent-sjc3-1.xx&oh=f382fc3680314fd576617cd6bd66f918&oe=5E60E4C8"
      title="Foto1"
      previewText="Descripcion foto 1"/>
      <Recipe
      thumbnail="https://scontent-sjc3-1.xx.fbcdn.net/v/t1.0-9/69329790_2427333307325793_8614874376166178816_n.jpg?_nc_cat=103&_nc_oc=AQkZ9cMASBt19z7o65gy109y7DPnsqkucDJIHO87eVP0ISJgMfei-4mgVb6H1hhTTnI&_nc_ht=scontent-sjc3-1.xx&oh=a45ec96c02540831fd1e5bf0652ae847&oe=5E516F35"
      title="Foto2"
      previewText="Descripcion foto 2"/>
  </section>
</template>

<script>
import Recipe from '@/components/Recipe'

export default {
  components: {
  Recipe
}
}
</script>
<style scoped>
.recipes {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-items: center;
}
</style>
