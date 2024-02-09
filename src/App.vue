<template>
  <div class="m-3" id="app">
    <SlideTabs>
      <SlideTab title="Tab 1">
        <div
          class="
            bg-blue-600
            h-[295px]
            text-xs
            leading-4
            text-white
            p-5
            gap-2
            rounded-3xl rounded-tl-none
          "
        >
          <div class="font-bold text-lg">Text 1</div>
          <div>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
            aliquip ex ea commodo consequat. Duis aute irure dolor in
            reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
            pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
            culpa qui officia deserunt mollit anim id est laborum
          </div>
        </div>
      </SlideTab>
      <SlideTab title="Tab 2">
        <div
          class="
            bg-blue-600
            h-[295px]
            text-xs
            leading-4
            text-white
            p-5
            rounded-3xl rounded-tl-none
          "
        >
          <div class="font-bold text-lg">Text 2</div>
          <div>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
            aliquip ex ea commodo consequat. Duis aute irure dolor in
            reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
            pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
            culpa qui officia deserunt mollit anim id est laborum
          </div>
        </div>
      </SlideTab>
      <SlideTab title="Tab 3">
        <div
          class="
            bg-blue-600
            h-[295px]
            text-xs
            leading-4
            text-white
            p-5
            rounded-3xl rounded-tl-none
          "
        >
          <div class="font-bold text-lg">Text 3</div>
          <div>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
            aliquip ex ea commodo consequat. Duis aute irure dolor in
            reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
            pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
            culpa qui officia deserunt mollit anim id est laborum
          </div>
        </div>
      </SlideTab>
    </SlideTabs>
  </div>
</template>

<script>
import SlideTab from './components/SlideTab.vue';
import SlideTabs from './components/SlideTabs.vue';

export default {
  name: 'App',
  components: {
    SlideTab,
    SlideTabs,
  },
};
</script>
