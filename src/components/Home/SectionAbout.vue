<template>
  <div class="container space-x-5">
    <div class="">
      <h2>Text about</h2>
      <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestiae
        voluptates nostrum tempora!
      </p>

      <br />
      <div class="row">
        <Card
          v-for="cardItem in cardItems"
          :key="cardItem.title"
          :title="cardItem.title"
          :description="cardItem.description"
        />
      </div>
    </div>
    <img src="" alt="" />
    <!-- to add image -->
  </div>
</template>

<script>
import Button from "../Buttons/Button.vue";
import Card from "../Cards/Card.vue";

export default {
  props: ["title", "type"],
  components: { Button, Card },
  setup() {
    const cardItems = [
      {
        title: "title 1",
        description: "lorem ipsum dolor sit amet",
      },
      {
        title: "title 2",
        description:
          "lorem ipsum dolor sit amet is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s",
      },
      {
        title: "title 3",
        description:
          "lorem ipsum dolor sit amet lorem ipsum dolor sit amet is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s",
      },
      {
        title: "title 4",
        description:
          "lorem ipsum dolor sit amet lorem ipsum dolor sit amet is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy",
      },
      {
        title: "title 5",
        description:
          "lorem ipsum dolor sit amet lorem ipsum dolor sit amet is simply dummy text",
      },
      {
        title: "title 6",
        description:
          "lorem ipsum dolor sit amet lorem ipsum dolor sit amet lorem ipsum dolor sit amet is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy",
      },
    ];

    return {
      cardItems,
    };
  },
};
</script>
