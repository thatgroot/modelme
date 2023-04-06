<script type="ts">
  import image_20 from "../../../assets/20.png";
  import line from "../../../assets/icons/line.svg";
  import Revolver from "../revolver.svelte";
</script>

<div
  id="intro"
  class="flex flex-col justify-start items-center self-stretch flex-grow-0 flex-shrink-0 overflow-hidden bg-white"
>
  <div
    class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative"
  >
    <div
      class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 relative gap-[94px]"
    >
      <div class="flex-grow-0 flex-shrink-0 w-[505px] h-[201px]">
        <span
          class="absolute left-0 -top-3 text-2xl font-semibold text-left text-[#1f206c]"
        >
          GENERATIVE SOFTWARE
        </span>
        <div
          class="flex flex-col justify-start items-start absolute left-0 top-[13px]"
        >
          <p
            class="flex-grow-0 flex-shrink-0 text-9xl text-left -tracking-[0.25rem]  text-neutral-900"
          >
            MODELME
          </p>

          <div
            class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 relative"
          >
            <span
              class="flex-grow-0 flex-shrink-0 w-[505px] text-lg text-left text-[#757575]"
            >
              The largest digital modeling agency in the world.
            </span>
            <span
              class="flex-grow-0 flex-shrink-0 w-[505px] text-lg text-left text-[#757575]"
            >
              Create more, with less.
            </span>
          </div>
        </div>
      </div>
      <div
        class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 relative"
      >
        <button
          class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-3 px-8 py-4 bg-[#1f206c]"
        >
          <span
            class="flex-grow-0 flex-shrink-0 text-lg font-medium text-left text-white"
          >
            Generate now
          </span>
          <svg
            width="25"
            height="25"
            viewBox="0 0 25 25"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            class="flex-grow-0 flex-shrink-0 w-6 h-6 relative"
            preserveAspectRatio="none"
          >
            <path
              d="M14.9297 6.57959L20.9997 12.6496L14.9297 18.7196"
              stroke="white"
              stroke-width="1.5"
              stroke-miterlimit="10"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
            <path
              d="M4 12.6494H20.83"
              stroke="white"
              stroke-width="1.5"
              stroke-miterlimit="10"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </svg>
        </button>
        <span
          class="flex-grow-0 flex-shrink-0 text-lg text-left text-[#757575]"
        >
          No credit card required.
        </span>
      </div>
    </div>
    <div
      class="flex-grow-0 flex-shrink-0 w-[710px] h-[636px] relative overflow-hidden"
      style="background: linear-gradient(134.88deg, #ececec -9.28%, rgba(236,236,236,0) 109.69%);"
    >
      <div class="w-[721px] h-[680px]">
        <div
          class="w-[138px] h-[638px] absolute left-[-7.5px] top-[-3.5px] bg-[#e3e2dd]"
        />
        <img
          src={image_20}
          alt="..."
          class="w-[610px] h-[677px] absolute left-[103.5px] top-[-0.5px] object-cover"
        />
      </div>
      <div
        class="flex flex-col justify-start items-start absolute left-[25px] top-[33px] gap-2"
      >
        <span
          class="flex-grow-0 flex-shrink-0 text-[22px] font-semibold text-left text-neutral-900"
        >
          Create more, with less
        </span>
        <span
          class="flex-grow-0 flex-shrink-0 text-lg text-left text-neutral-900"
        >
          Fashion e-Comm
        </span>
        <span
          class="flex-grow-0 flex-shrink-0 opacity-50 text-sm text-left text-neutral-900"
        >
          by Frankie’s Shop
        </span>
      </div>
    </div>
  </div>
  <Revolver />
</div>
