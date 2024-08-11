<template>
  <learning-resource
    v-for="res in storedResources"
    :key="res.id"
    :title="res.title"
    :description="res.description"
    :link="res.link"
  ></learning-resource>
</template>

<script>
export default {
  props: ['resources'],
};
</script>
