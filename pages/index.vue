<template>
<div>
<h1>{{ date }}</h1>
<div class="one">123</div>
</div>

</template>

<script>

export default {
 name: 'date',
  serverCacheKey() {
    // Will change every 10 secondes
    return Math.floor(Date.now() / 10000)
  },
  data() {
    return { date: Date.now() }
  }
 

}
</script>

<style>

</style>
