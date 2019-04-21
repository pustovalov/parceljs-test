<template>
  <div>
    <ul class="list-unstyled links custom-links">
      <li v-for="link in links">
        <a :href="link.url" target="_blank">{{ link.title }}</a>
      </li>
      <!-- <li>
        <a href="/1.pdf" target="_blank">test</a>
      </li>-->
    </ul>
  </div>
</template>

<script>
import { mapGetters, mapActions } from 'vuex'

export default {
  computed: {
    ...mapGetters('main', ['links']),
  },
}
</script>
