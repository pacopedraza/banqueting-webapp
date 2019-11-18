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
              title: "Pollo a las finas hiervas",
              previewText: "Acompañado de una deliciosa salsa de chipotle",
              thumbnail: "https://scontent-sjc3-1.xx.fbcdn.net/v/t1.0-9/67663359_2398087150250409_6330050507402379264_o.jpg?_nc_cat=109&_nc_oc=AQm5yyJVB88vYL1YfZg-_YK0DtV30kJTb-sgSXOL0sSQl3nx52k7sYnCq6Dd25f5QuY&_nc_ht=scontent-sjc3-1.xx&oh=d43d5f8839309580634b28d2369b5111&oe=5E8BDAC0"
            },
            {
              id: "2",
              title: "Graduación Universidad X",
              previewText: "Carpa arabe",
              thumbnail: "https://scontent-sjc3-1.xx.fbcdn.net/v/t1.0-9/69329790_2427333307325793_8614874376166178816_n.jpg?_nc_cat=103&_nc_oc=AQkZ9cMASBt19z7o65gy109y7DPnsqkucDJIHO87eVP0ISJgMfei-4mgVb6H1hhTTnI&_nc_ht=scontent-sjc3-1.xx&oh=a45ec96c02540831fd1e5bf0652ae847&oe=5E516F35"
            },
            {
              id: "3",
              title: "Arreglo floral",
              previewText: "Boda de Dany X",
              descriptionText: "Salon X",
              thumbnail: "https://scontent-sjc3-1.xx.fbcdn.net/v/t1.0-9/67609094_2395746507151140_5410490411531632640_o.jpg?_nc_cat=103&_nc_oc=AQmn4JloioQQ2OOEfqzgYy2aUXFYvJGDIuRKxeQOyF68cENwbaFGbiqv7mulv6zmH1g&_nc_ht=scontent-sjc3-1.xx&oh=ecbe0f9c1d402ab035a552b0df6e4211&oe=5E4270C4"
            },
            {
              id: "4",
              title: "Graduación Enfermería",
              previewText: "Salón Y",
              descriptionText: "Generación 2017-2019",
              thumbnail: "https://scontent-sjc3-1.xx.fbcdn.net/v/t1.0-9/67514969_2395746210484503_2393334774388228096_o.jpg?_nc_cat=111&_nc_oc=AQltXa-62P3M1ObqgwTz59zICzWCLM_z05SVGlA1qFycgRSFFIIj4pN1KRe4JmdHChw&_nc_ht=scontent-sjc3-1.xx&oh=fb6a66cadec95f5caf0bf00042763c9b&oe=5E8645A3"
            },
            {
              id: "5",
              title: "XV Años",
              previewText: "Silla Tiffany",
              descriptionText: "Salon X",
              thumbnail: "https://scontent-sjc3-1.xx.fbcdn.net/v/t1.0-9/67935607_2392617644130693_7994615011961995264_o.jpg?_nc_cat=109&_nc_oc=AQlR_AFAWfXMmY3s56ZFww0V1LlrKwbs7xEd3TLONLaFw5zH2YJ7muFIHMu6UuQlQ44&_nc_ht=scontent-sjc3-1.xx&oh=757f8e6a246e9583a4fff22d91efcc56&oe=5E53D6F9"
            },
            {
              id: "6",
              title: "Graduación Ing x",
              previewText: "Universidad de Guanajuato",
              descriptionText: "Generación 2016-2019",
              thumbnail: "https://scontent-sjc3-1.xx.fbcdn.net/v/t1.0-9/66505008_2360123137380144_2458948027696545792_o.jpg?_nc_cat=100&_nc_oc=AQmm8smS1GEdIf9xgBlTLAqWZcK5PbcOx1MmGVNBe2DkSZGZSJccCbQw4g36S2UtIIg&_nc_ht=scontent-sjc3-1.xx&oh=a0010b513af0e9ff6b3b34549f8e56e8&oe=5E83AD74"
            },
            {
              id: "7",
              title: "Boda Luis y Lupita",
              previewText: "Hacienda X",
              descriptionText: "Arreglo con hermosa carpa arabe",
              thumbnail: "https://scontent-sjc3-1.xx.fbcdn.net/v/t1.0-9/66020722_2342994009093057_4329691775875678208_o.jpg?_nc_cat=106&_nc_eui2=AeGWguAqMA_J0plly3gTaVOVrxydF7IrH34gi-CjfBkdamFhJ0eE5liDaxnmwTp8DsJ4yYVXtmhjAG3_h-vFLCQlGUeDgUrvfUkhuyDyb4nYUw&_nc_oc=AQkFNqv4GMGXs74dCxK6Em497KLz8pHOkpQRkiF8DfmTmvp0bdrooL1axEfv4fJpRJE&_nc_ht=scontent-sjc3-1.xx&oh=b66f5f1b76d397ac67f83f7ed806ac22&oe=5E87FFBF"
            },
            {
              id: "8",
              title: "Graduación Licenciatura",
              previewText: "Universidad de Guanajuato",
              descriptionText: "Generación 2016-2019",
              thumbnail: "https://scontent-sjc3-1.xx.fbcdn.net/v/t1.0-9/65103217_2328764893849302_8438146427669970944_o.jpg?_nc_cat=101&_nc_eui2=AeFmJtwUEyunjy0NlnN8R4R6TWGVCNbIPFF9fzFr5GpdIdPGJb-NtxCzcrR5u_GGy9GGnFMl6xzO8ru_5L7TYlL4IRXCHzWcEu9VCgdi7pIbRA&_nc_oc=AQmURZE9UegGXg_YxMZbynU069bx2CKb0flQlaB86mhwBwsT_esPIVfdPhsizXIslJA&_nc_ht=scontent-sjc3-1.xx&oh=8b8af83072115223646b5d09978fc25b&oe=5E5001AE"
            },
            {
              id: "9",
              title: "Pinturas Berel",
              previewText: "Evento empresarial",
              descriptionText: "Uno de nuestros clientes más fieles y mas queridos",
              thumbnail: "https://scontent-sjc3-1.xx.fbcdn.net/v/t1.0-9/52938301_2146844568708003_4893266896146661376_o.jpg?_nc_cat=107&_nc_eui2=AeEDYbQgEGfZteRL0MvD2XUjfkOD24r8nRV67lZgOQBduyOm9aRHsL5HfSpkWsbCDrTXbvB3JSzRREcN3z19DsrbMPe5Trf83lU_xQO5ksBTeQ&_nc_oc=AQnsL6L5DrKH8o5qoa-IRtC8vg1oqNCBdaXM48sUPm_0Vj7pXaY4qOdELw68Rw27YSk&_nc_ht=scontent-sjc3-1.xx&oh=36b108ff2ccfa0a2560d32cb2d56b88a&oe=5E3ECAEC"
            },
            {
              id: "10",
              title: "BBVA",
              previewText: "Evento empresarial",
              descriptionText: "Fiesta anual BBVA",
              thumbnail: "https://scontent-sjc3-1.xx.fbcdn.net/v/t1.0-9/51584433_2108962592496201_7930085400377294848_o.jpg?_nc_cat=108&_nc_eui2=AeFaeGkS_i1Looe-tIF6oWd4PWr2r4WMjB0n5zIgP4HvX9ynKWhUz-cmt4dgukcYFaxg8_Bes_AkBpV25__nXZ0CTL2rS3UKyz3SbmEJlOc5-Q&_nc_oc=AQnGpdwq_IxFniWsD-e6Y_5RIiH5tbi57VGedyEVi0B8RyJ30aMlwlhYEECi3LMEcWE&_nc_ht=scontent-sjc3-1.xx&oh=8988b07b3eb438e6ef8a68dcf7e2c38b&oe=5E852C85"
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
