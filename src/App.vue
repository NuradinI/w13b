<template>
  <div id="app">
    <page-header></page-header>
    <user-tweet></user-tweet>
  </div>
</template>

<script>
import UserTweet from './components/tweet.vue'
import PageHeader from './components/page-header.vue'

export default {
  name: 'App',
  components: {
    UserTweet,
    PageHeader
  }
}
</script>

<style>

</style>
