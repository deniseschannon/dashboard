<script>
import Loading from '@/components/Loading';

export default {
  components: { Loading },

  data: () => ({ loading: false }),

  methods:    {
    start() {
      this.loading = true;
    },
    finish() {
      this.loading = false;
    }
  }
};

</script>
<template>
  <Loading v-if="loading" />
</template>
