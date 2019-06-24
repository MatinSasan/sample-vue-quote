<template>
  <div class="col-sm-6 col-md-4 col-lg-3">
    <div class="panel panel-default">
      <div class="panel-body quote">
        <slot></slot>
      </div>
    </div>
  </div>
</template>

<script>
</script>

<style>
.panel-body {
  font-family: "Slabo 27px", cursive;
  font-size: 24px;
  color: #34495e;
}

.quote {
  cursor: pointer;
}
.quote:hover {
  background-color: #41b883;
  color: whitesmoke;
}
</style>
