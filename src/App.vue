<template>
  <div id='app'>
    <button @click='state = "walk"'>Walk</button>
    <button @click='state = "attack"'>Attack</button>
    <button @click='state = "die"'>Die</button>

    <knight :state=state></knight>
  </div>
</template>

<script>
import Knight from '@/components/Knight'

export default {
  name: 'app',
  data () {
    return { state: 'walk' }
  },
  components: { Knight }
}
</script>
