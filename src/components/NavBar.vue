<template>
  <q-list>
    <q-item v-for="info in navInfo" :key="info.id" clickable tag="a" target="_blank" :href="info.link">
      <q-item-section avatar>
        <q-icon :name="info.icon" />
      </q-item-section>
      <q-item-section>{{info.title}}</q-item-section>
    </q-item>
  </q-list>
</template>

<script>
export default {
  name: 'NavBar',
  data () {
    return {
      navInfo: [
        { title: 'Personal Site v1', icon: 'construction', link: 'https://alexgrahamross.ca/' },
        { title: 'Github', icon: 'person', link: 'https://github.com/alexross93' }
      ]
    }
  }
}
</script>
