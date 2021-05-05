<template>
  <div>
    <h1>Jobs</h1>
    <div v-for="job in jobs" :key="job.id">
      <router-link :to="{ name: 'JobsDetails', params: { id: job.id } }">
        <h2>{{ job.title }}</h2>
      </router-link>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      jobs: [
        { title: "Ninja UX Designer", id: 1, details: "lorem" },
        { title: "Ninja web Designer", id: 2, details: "lorem" },
        { title: "Ninja vue Designer", id: 3, details: "lorem" },
      ],
    };
  },
};
</script>

<style lang="scss" scoped></style>
