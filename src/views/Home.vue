<template>
  <div>
    {{name}}
  </div>
</template>

<script>
import { mapGetters} from 'vuex'
export default {
  computed: {
    ...mapGetters([
      'name',
    ]),
  },
  data () {
    return {
      num:2
    }
  }
}
</script>
