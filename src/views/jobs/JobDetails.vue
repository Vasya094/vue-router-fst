<template>
  <div>
    <h1>Job Details Page</h1>
    <p>The job id is {{ $route.params.id }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      info: this.$route,
    };
  },
  mounted() {
    console.log(this.info);
  },
};
</script>

<style lang="scss" scoped></style>
