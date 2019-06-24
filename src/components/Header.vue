<template>
  <div class="row">
    <div class="col-sm-12">
      <h3>Quotes Added</h3>
      <div class="progress">
        <div
          class="progress-bar"
          role="progressbar"
          aria-valuenow="60"
          aria-valuemin="0"
          aria-valuemax="100"
          :style="[
          {width: (quoteCount / maxQuotes) * 100 + '%'},
           {background: 'rgb(2,0,36)'},
           {background: 'linear-gradient(90deg, rgba(2,0,36,1) 0%, rgba(52,73,94,1) 15%, rgba(65,184,131,1) 100%)'}
           ]"
        >{{quoteCount}} / {{maxQuotes}}</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["quoteCount", "maxQuotes"]
};
</script>

