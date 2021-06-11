<template>
    <div>
      <PetTable species="dogs" :pets="dogs" />
    </div>
</template>
<script>
import { mapState } from 'vuex'
import PetTable from '@/components/PetTable.vue'
export default {
  components: {
    PetTable
  },
  computed: { ...mapState(['dogs']) }
}
</script>
