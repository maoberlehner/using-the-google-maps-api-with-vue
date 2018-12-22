<template>
  <div class="App"/>
</template>

<script>
import gmapsInit from './utils/gmaps';

export default {
  name: `App`,
  async mounted() {
    try {
      const google = await gmapsInit();
      console.log(google);
    } catch (error) {
      console.error(error);
    }
  },
};
</script>
