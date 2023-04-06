<script lang="ts">
  // @ts-nocheck

  import { onMount } from "svelte";

  export let min: number = 0;
  export let max: number = 12;
  let val: number = 8;

  onMount(() => {
    let slider = document.getElementById("slider");
    let selector = document.getElementById("selector");
    let selectValue = document.getElementById("selectValue");
    let progressBar = document.getElementById("progressBar");

    selectValue.innerHTML = slider.value;

    slider.oninput = function () {
      // percentage of value out of 12
      const _value = Math.ceil((this.value / 12) * 100);
      selectValue.innerHTML = this.value;
      selector.style.left = _value + "%";
      progressBar.style.width = _value + "%";
    };
  });
</script>

<div class="flex flex-col gap-2 w-full">
  <div class="flex justify-between">
    <span class="text-left text-base font-medium text-[#492c2c]">
      {min}
    </span>
    <span class="text-left text-base font-medium text-[#232323]">
      {max}
    </span>
  </div>
  <!--  -->
  <!--  -->
  <div class="w-full relative">
    <input
      type="range"
      min="0"
      max="12"
      value="8"
      id="slider"
      class="appearance-none w-full h-[7px] rounded-sm"
    />
    <div id="selector" class="w-12 h-12 absolute -bottom-5 left-[50%] z-[2]">
      <div class="selectBtn" />
      <div
        class="flex absolute -left-[22px] right-0 -top-[30px] mx-auto w-fit flex-col items-start justify-start gap-2.5 bg-[#232323] px-3 py-1"
      >
        <span
          id="selectValue"
          class="flex-shrink-0 flex-grow-0 text-left text-base font-medium text-white"
        >
          {val}
        </span>
      </div>
    </div>
    <div id="progressBar" />
    <div id="progressBar2" />
  </div>
</div>

<style>
  /* Design slider button */
  #slider::-webkit-slider-thumb {
    -webkit-appearance: none;
    width: 48px;
    height: 48px;
    cursor: pointer;
    position: relative;
    z-index: 3;
  }

  .selectBtn {
    height: 24px;
    width: 24px;
    background-image: url(/track.svg);
    background-repeat: no-repeat;
    background-size: cover;
    position: absolute;
    bottom: 15px;
  }
  #progressBar {
    width: 50%;
    height: 4px;
    background: #1f206c;
    border-radius: 3px;
    position: absolute;
    bottom: 4px;
    left: 0;
    z-index: 9999;
  }
  #progressBar2 {
    width: 100%;
    height: 4px;
    background: #aeaeae;
    border-radius: 3px;
    position: absolute;
    bottom: 4px;
    left: 0;
  }
</style>
