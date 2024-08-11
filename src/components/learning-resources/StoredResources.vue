<template>
  <learning-resource
    v-for="res in resources"
    :key="res.id"
    :title="res.title"
    :description="res.description"
    :link="res.link"
  ></learning-resource>
</template>

<script>
import LearningResource from './LearningResource.vue';

export default {
  props: ['resources'],
  components: {
    LearningResource,
  },
};
</script>
