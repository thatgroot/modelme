<script lang="ts">
  import image_37 from "../../../assets/37.png";
  import image_38 from "../../../assets/38.png";
  import image_39 from "../../../assets/39.png";
  import SubscriptionOverlay from "../subscription-overlay.svelte";
</script>

<div
  id="pricing"
  class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 overflow-hidden gap-[60px] px-[68px] pt-[100px] pb-6 bg-white border-t-0 border-r-0 border-b border-l-0 border-[#232323]/[0.16]"
>
  <div
    class="flex justify-start items-start flex-grow-0 flex-shrink-0 relative gap-[222px]"
  >
    <div
      class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 relative gap-6"
    >
      <p
        class="flex-grow-0 flex-shrink-0 text-lg font-semibold text-left text-[#1f206c]"
      >
        PRICING
      </p>
      <p
        class="flex-grow-0 flex-shrink-0 text-[58px] text-left text-neutral-900"
      >
        It’s all about the grade
      </p>
    </div>
    <p
      class="flex-grow-0 flex-shrink-0 w-[610px] text-lg text-left text-[#757575]"
    >
      Revolutionising visual content creation through intuitive and affordable
      software for all. We recommend you first test our software with our free
      trial.
    </p>
  </div>
  <div
    class="flex flex-col justify-start items-center flex-grow-0 flex-shrink-0 gap-[46px]"
  >
    <div
      class="flex justify-center items-center flex-grow-0 flex-shrink-0 h-[571px] gap-6"
    >
      <div
        class="group flex flex-col justify-start items-center self-stretch flex-grow-0 flex-shrink-0 w-[408px] relative overflow-hidden gap-[25px] bg-[#e3e4dd]"
      >
        <div
          class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 relative group-hover:opacity-0"
        >
          <p
            class="flex-grow-0 flex-shrink-0 text-[32px] font-semibold text-left text-neutral-900"
          >
            Entry Grade (EG)
          </p>
          <p
            class="flex-grow-0 flex-shrink-0 text-[32px] font-semibold text-left text-neutral-900"
          >
            €10/mo | €96/yr
          </p>
        </div>
        <img
          src={image_37}
          alt="..."
          class="flex-grow w-[408px] object-cover group-hover:blur-3xl"
        />

        <SubscriptionOverlay />
      </div>
      <div
        class="flex group flex-col justify-start items-center self-stretch flex-grow-0 flex-shrink-0 w-[408px] relative overflow-hidden gap-[11px] py-1 bg-[#d3d7cc]"
      >
        <div
          class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 relative group-hover:opacity-0"
        >
          <p
            class="flex-grow-0 flex-shrink-0 text-[32px] font-semibold text-left text-neutral-900"
          >
            High Grade (HG)
          </p>
          <p
            class="flex-grow-0 flex-shrink-0 text-[32px] font-semibold text-left text-neutral-900"
          >
            €30/mo | €288/yr
          </p>
        </div>
        <img
          src={image_38}
          alt="..."
          class="flex-grow w-[447px] object-cover  group-hover:blur-3xl"
        />
        <SubscriptionOverlay />

      </div>
      <div
        class="flex group flex-col justify-start items-center self-stretch flex-grow-0 flex-shrink-0 w-[408px] relative overflow-hidden bg-[#d3d7cc]"
      >
        <div
          class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 relative group-hover:opacity-0"
        >
          <p
            class="flex-grow-0 flex-shrink-0 text-[32px] font-semibold text-left text-neutral-900"
          >
            Real Grade (RG)
          </p>
          <p
            class="flex-grow-0 flex-shrink-0 text-[32px] font-semibold text-left text-neutral-900"
          >
            €60/mo | €576/yr
          </p>
        </div>
        <img
          src={image_39}
          alt="..."
          class="flex-grow w-[468px] object-cover  group-hover:blur-3xl"
        />
        <SubscriptionOverlay />

      </div>
    </div>
    <div
      class="flex justify-center items-center flex-grow-0 flex-shrink-0 relative gap-3"
    >
      <p class="flex-grow-0 flex-shrink-0 text-lg text-left text-[#757575]">
        Contact us for custom plans that require a higher limit or special
        requirements.
      </p>
      <div
        class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-3 px-8 py-4 bg-white border border-[#1f206c]"
      >
        <p
          class="flex-grow-0 flex-shrink-0 text-lg font-medium text-left text-[#1f206c]"
        >
          Contact us
        </p>
        <svg
          width="24"
          height="25"
          viewBox="0 0 24 25"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          class="flex-grow-0 flex-shrink-0 w-6 h-6 relative"
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
