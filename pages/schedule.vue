<script lang="ts" setup>
definePageMeta({
  layout: 'default',
})

const activeDay = ref('day1')

function showDayX(component: string) {
  activeDay.value = component
}
</script>

<template>
  <div class="lg:ml-30 mx-5 mt-10 md:ml-44">
    <div class="mb-20">
      <p class="mb-5 text-3xl font-bold md:text-5xl">
        PROGRAMAÇÃO
      </p>
      <p class="max-w-sm text-xl md:max-w-md">
        A 7º edição do ENCOMP vai ocorrer nos dias 06, 07 e 08 de novembro, confira nossa programação
      </p>
      <div class="mt-4 flex gap-3">
        <Button
          variant="default"
          class="bg-tertiary text-white"
          @click="showDayX('day1')"
        >
          06/11
        </Button>
        <Button
          variant="default"
          class="bg-tertiary text-white"
          @click="showDayX('day2')"
        >
          07/11
        </Button>
        <Button
          variant="default"
          class="bg-tertiary text-white"
          @click="showDayX('day3')"
        >
          08/11
        </Button>
      </div>
    </div>
    <div>
      <ScheduleDay1 v-if="activeDay === 'day1'" />
      <ScheduleDay2 v-if="activeDay === 'day2'" />
      <ScheduleDay3 v-if="activeDay === 'day3'" />
    </div>
  </div>
</template>
