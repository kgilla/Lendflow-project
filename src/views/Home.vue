<template>
  <div class="home">
    <h3>hello world</h3>
  </div>
</template>

<script>
export default {
  name: "Home",
  // components: {
  //   HelloWorld,
  // },
  setup() {
    fetch("https://api.github.com/organizations").then((res) =>
      res.json().then((data) => console.log(data))
    );
  },
};
</script>
