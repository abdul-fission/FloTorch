<script setup lang="ts">

const meta = useProjectCreateMeta()

const regions = computed(() => {
  return meta.dataStrategy.regions
})

</script>



<template>
  <USelectMenu :items="regions" class="w-full" value-key="value" />
</template>
