<script lang="ts">
  import arrow_right from "../../assets/icons/arrow-right.svg";
  import Badge from "./badge.svelte";
  export let active: boolean = false;
</script>

<div
  class="absolute left-0 right-0 top-0 bottom-0 {active
    ? 'block'
    : 'hidden'} group-hover:block"
  style="background: linear-gradient(134.88deg, #ececec -9.28%, rgba(236,236,236,0) 109.69%);"
>
  <div class="relative overflow-hidden w-full h-full">
    <div
      class="w-full h-[582px] absolute left-[-1px] top-[-1px] bg-gradient-to-b from-[#4434c9]/80 to-[#4434c9]/0"
    />
    <div
      class="flex flex-col justify-start items-center absolute left-10 top-[41px] gap-[123px]"
    >
      <div class="flex flex-col justify-start items-start gap-12">
        <div class="flex flex-col justify-start items-start relative">
          <span
            class="text-[32px] font-semibold text-left text-white leading-[39px]"
          >
            Entry Grade (EG)
          </span>
          <span class="text-[32px] font-semibold text-left text-white">
            €10/mo | €96/yr
          </span>
          <span class="text-lg text-left text-white leading-3">
            Save 20% on yearly plans
          </span>
        </div>
        <div class="flex flex-col justify-start items-start relative gap-0.5">
          <span class="w-[312px] text-lg text-left text-white">
            1,000 fast generations per month.
          </span>
          <span class="w-[312px] text-lg text-left text-white">
            2 parallel fast generations.
          </span>
          <span class="w-[312px] text-lg text-left text-white">
            Commercial license (solo).
          </span>
          <span class="w-[312px] text-lg text-left text-white">
            Images are public.
          </span>
          <span class="w-[312px] text-lg text-left text-white">
            No slow generations.
          </span>
        </div>
      </div>
      <div
        class="flex justify-center items-center w-[312px] relative gap-3 px-8 py-4 bg-white"
      >
        <span class="text-lg font-medium text-left text-[#1f206c]">
          Subscribe
        </span>
        <img src={arrow_right} alt="arrow_right" class="w-6 h06 relative" />
        <slot />
      </div>
    </div>
  </div>
</div>
