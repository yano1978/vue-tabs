<template>
  <div>
    <ul
      class="
        flex flex-wrap
        [&_button]:items-center
        [&_button]:justify-center
        [&_button]:w-40
        [&_button]:h-10
      "
    >
      <li
        class="mr-2 transition-transform ease-in-out delay-150"
        :class="{ selected: title == selectedTitle }"
        @click="selectedTitle = title"
        v-for="title in tabTitles"
        :key="title"
      >
        <button
          :datatype="title"
          class="
            inline-flex
            font-bold
            bg-gray
            text-blue-light
            rounded-lg
            py-1
            px-2
            text-sm text-center
            leading-4
          "
        >
          {{ title }}
        </button>
      </li>
    </ul>
    <slot />
  </div>
</template>
<script>
import { ref, provide } from 'vue';
export default {
  setup(props, { slots }) {
    const tabTitles = ref(slots.default().map((tab) => tab.props.title));
    const selectedTitle = ref(tabTitles.value[0]);
    provide('selectedTitle', selectedTitle);
    return { tabTitles, selectedTitle };
  },
};
</script>
<style lang="postcss">
.selected {
  button {
    background-color: rgb(37 99 235);
    color: #fff;
    border-top-left-radius: 10px;
    border-top-right-radius: 10px;
    border-bottom-left-radius: 0;
    border-bottom-right-radius: 0;
  }
}
</style>
