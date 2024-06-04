<template>
  <div>
    <Suspense>
      <AsyncCityView />
      <template #fallback>
        <CityViewSketelon />
      </template>
    </Suspense>
  </div>
</template>

<script setup>
import CityViewSketelon from '../components/app-components/CityViewSkeleton.vue'
import AsyncCityView from '../components/app-components/AsyncCityView.vue'
</script>

<style lang="scss" scoped></style>
