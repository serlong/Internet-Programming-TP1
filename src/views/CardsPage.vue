<template>
  <div class="Cards-Row">
    <Cards
      v-for="i in Cards"
      :key="i.Cards"
      :bg="i.bg"
      :Img="i.Img"
      :Text="i.Text"
      :bgBtn="i.btncolor"
      :TextBtn="i.TextBtn" />
  </div>
</template>

<script>
import Cards from "../components/Cards.vue";
import Buttons from "../components/Buttons.vue";
import Img1 from "../assets/images/berry bottle.png";
import Img2 from "../assets/images/onion.png";
import Img3 from "../assets/images/veg.png";
export default {
  name: "CardsProduct",
  components: {
    Cards,
    Buttons,
  },
  data() {
    return {
      Cards: [
        {
          Text: "Everyday Fresh & Clean with Our Products",
          Img: Img2,
          btncolor: "rgba(59, 183, 126, 1)",
          TextBtn: "Shop Now",
        },
        {
          Text: "Make your Breakfast Healthy and Easy",
          Img: Img1,
          bg: "rgba(243, 232, 232, 1)",
          btncolor: "rgba(205, 50, 17, 1)",
          TextBtn: "Shop Now",
        },
        {
          Text: "The Best Organic Products Online",
          Img: Img3,
          bg: "rgba(231, 234, 243, 1)",
          btncolor: "rgba(253, 192, 64, 1)",
          TextBtn: "Shop Now",
        },
      ],
    };
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Kantumruy+Pro:ital,wght@1,300;1,400;1,500;1,600;1,700&family=Poppins:wght@300;400;500;600;800&family=Quicksand:wght@400;600;700&display=swap");

.Cards-Row {
  width: 100%;
  display: flex;
  justify-content: start;
  align-items: center;
  gap: 15px;
}
</style>
