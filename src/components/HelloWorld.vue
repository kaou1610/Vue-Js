<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p class="intro">{{intro}}</p>
    <span class="content">
      <div class="icon">
        <font-awesome-icon icon="spinner" />
      </div>
      <div class="price">
        <span>
          <h4>Anual</h4>
          <p>$55.99/year</p>
        </span>
      </div>
      <div class="change"><a href="Change">Change</a></div>
    </span>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      intro: 'You can now listen to millions of songs audiobooks and podcasts on any device anywhere you like!'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.intro {
  opacity: 0.7;
  padding: 10px 60px;
}
.content {
  background-color: rgba(244, 239, 248, 0.918);
  width: 70%;
  margin: auto;
  border-radius: 10px;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-evenly;
}
</style>
