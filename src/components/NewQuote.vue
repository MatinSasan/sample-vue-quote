<template>
  <div class="row">
    <form action>
      <div class="col-sm-8 col-sm-offset-2 col-xs-12 col-md-offset-3 form-group">
        <label>Quote</label>
        <textarea class="form-control" rows="3" v-model="quote"></textarea>
      </div>
      <div class="col-sm-8 col-sm-offset-2 col-xs-12 col-md-offset-3 form-group">
        <button class="btn" @click.prevent="createNew">Add Quote</button>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      quote: ""
    };
  },
  methods: {
    createNew() {
      this.$emit("newQuote", this.quote);
      this.quote = "";
    }
  }
};
</script>

<style>
button {
  background-color: #34495e;
  color: whitesmoke;
}
button:hover {
  background-color: #41b883;
  color: whitesmoke;
}
</style>
