<script lang="ts">
  import image_37 from "../../../assets/37.png";
  import image_38 from "../../../assets/38.png";
  import image_39 from "../../../assets/39.png";
  import Badge from "../badge.svelte";
  import SubscriptionOverlay from "../subscription-overlay.svelte";
</script>

<div
  id="pricing"
  class="flex flex-col justify-start items-start overflow-hidden gap-[60px] px-[68px] pt-[100px] pb-6 bg-white border-t-0 border-r-0 border-b border-l-0 border-[#232323]/[0.16]"
>
  <div class="flex justify-start items-start relative gap-[222px]">
    <div class="flex flex-col justify-start items-start relative gap-6">
      <span class="text-lg font-semibold text-left text-[#1f206c]">
        PRICING
      </span>
      <p class="text-[58px] text-left text-neutral-900 tracking-tight">
        It’s all about the grade
      </p>
    </div>
    <span class="w-[610px] text-lg text-left text-[#757575]">
      Revolutionising visual content creation through intuitive and affordable
      software for all. We recommend you first test our software with our free
      trial.
    </span>
  </div>
  <div class="flex flex-col justify-start items-center gap-[46px]">
    <div class="flex justify-center items-center h-[600px] gap-6">
      <div
        class="group flex flex-col justify-start items-center self-stretch w-[408px] p-10 relative overflow-hidden gap-[25px] bg-[#e3e4dd]"
      >
        <div
          class="flex flex-col justify-start items-start relative group-hover:opacity-0"
        >
          <span class="text-[32px] font-semibold text-left text-neutral-900 leading-[39px]">
            Entry Grade (EG)
          </span>
          <span class="text-[32px] font-semibold text-left text-neutral-900">
            €10/mo | €96/yr
          </span>
        </div>
        <img
          src={image_37}
          alt="..."
          class="absolute -bottom-10 pt-4 z-0 object-cover group-hover:blur-3xl"
        />

        <SubscriptionOverlay />
      </div>
      <div
        class="group flex flex-col justify-start items-center self-stretch w-[408px] p-10 relative overflow-hidden gap-[25px] bg-[#e3e4dd]"
      >
        <div
          class="flex flex-col justify-start items-start relative group-hover:opacity-0"
        >
          <span class="text-[32px] font-semibold text-left text-neutral-900 leading-[39px]">
            High Grade (HG)
          </span>
          <span class="text-[32px] font-semibold text-left text-neutral-900">
            €30/mo | €288/yr
          </span>
        </div>
        <img
          src={image_38}
          alt="..."
          class="absolute -bottom-10 pt-4 z-0 object-cover group-hover:blur-3xl"
        />
        <SubscriptionOverlay>
          <div class="absolute -bottom-7 -right-8">
            <Badge lable="Most popular" />
          </div>
        </SubscriptionOverlay>
      </div>
      <div
        class="group flex flex-col justify-start items-center self-stretch w-[408px] p-10 relative overflow-hidden gap-[25px] bg-[#e3e4dd]"
      >
        <div
          class="flex flex-col justify-start items-start relative group-hover:opacity-0"
        >
          <span class="text-[32px] font-semibold text-left text-neutral-900 leading-[39px]">
            Real Grade (RG)
          </span>
          <span class="text-[32px] font-semibold text-left text-neutral-900">
            €60/mo | €576/yr
          </span>
        </div>
        <img
          src={image_39}
          alt="..."
          class="absolute -bottom-10 pt-4 z-0 object-cover group-hover:blur-3xl"
        />
        <SubscriptionOverlay>
          <div class="absolute -bottom-7 -right-8">
            <Badge lable="Best value" />
          </div>
        </SubscriptionOverlay>
      </div>
    </div>
    <div class="flex justify-center items-center relative gap-3">
      <span class="text-lg text-left text-[#757575]">
        Contact us for custom plans that require a higher limit or special
        requirements.
      </span>
      <div
        class="flex justify-start items-center relative gap-3 px-8 py-4 bg-white border border-[#1f206c]"
      >
        <span class="text-lg font-medium text-left text-[#1f206c]">
          Contact us
        </span>
        <svg
          width="24"
          height="25"
          viewBox="0 0 24 25"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          class="w-6 h-6 relative"
          preserveAspectRatio="none"
        >
          <path
            d="M14.4297 6.57941L20.4997 12.6494L14.4297 18.7194"
            stroke="#1F206C"
            stroke-width="1.5"
            stroke-miterlimit="10"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M3.5 12.6494H20.33"
            stroke="#1F206C"
            stroke-width="1.5"
            stroke-miterlimit="10"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>
      </div>
    </div>
  </div>
</div>
