<script lang="ts">
  import { createEventDispatcher } from "svelte";
  import image_14 from "../../../assets/14.png";
  import divider_svg from "../../../assets/icons/divider.svg";

  const dispatch = createEventDispatcher();
</script>

<!-- svelte-ignore a11y-click-events-have-key-events -->
<div
  class="z-[999] fixed top-0 left-0 bottom-0 right-0 bg-[#232323]/50 flex flex-col justify-center items-center w-full"
>
  <div
    on:click={() => {
      dispatch("close");
    }}
    class="flex flex-col justify-center items-center absolute left-0 top-0 right-0 bottom-0 gap-6 p-8 bg-[#232323]/50"
  />
  <div
    class="z-[999] flex justify-start items-start gap-9 px-[51px] py-[31px] bg-white"
  >
    <div class="flex flex-col justify-start items-start gap-[41px]">
      <div class="flex justify-start items-start w-[360px] relative gap-6">
        <span
          class="flex-grow font-semibold w-[312px] text-[32px] leading-[38.4px] -tracking-[1.1px] text-left text-[#232323]"
        >
          Lorem ipsum dolor sit amet consectetur.
        </span>
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
            d="M13.2594 4.09997L5.04936 12.79C4.73936 13.12 4.43936 13.77 4.37936 14.22L4.00936 17.46C3.87936 18.63 4.71936 19.43 5.87936 19.23L9.09936 18.68C9.54936 18.6 10.1794 18.27 10.4894 17.93L18.6994 9.23997C20.1194 7.73997 20.7594 6.02997 18.5494 3.93997C16.3494 1.86997 14.6794 2.59997 13.2594 4.09997Z"
            stroke="#9A9A9A"
            stroke-width="1.5"
            stroke-miterlimit="10"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M11.8906 5.55005C12.3206 8.31005 14.5606 10.42 17.3406 10.7"
            stroke="#9A9A9A"
            stroke-width="1.5"
            stroke-miterlimit="10"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M3 22.5H21"
            stroke="#9A9A9A"
            stroke-width="1.5"
            stroke-miterlimit="10"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>
      </div>
      <div class="flex flex-col justify-start items-start gap-6">
        <div class="flex justify-start items-start w-[408px] gap-4">
          <div
            class="flex flex-col justify-start items-start w-[145px] relative gap-1"
          >
            <p class="text-sm text-left text-[#9a9a9a]">Visbility</p>
            <p class="text-base font-medium text-left text-[#232323]">Public</p>
          </div>
          <div
            class="flex flex-col justify-start items-start flex-grow relative gap-1"
          >
            <p class="text-sm text-left text-[#9a9a9a]">License</p>
            <p class="text-base font-medium text-left text-[#232323]">
              Non Commercial License
            </p>
          </div>
        </div>
        <div class="flex justify-start items-start w-[408px] gap-4">
          <div
            class="flex flex-col justify-start items-start w-[145px] relative gap-1"
          >
            <p class="text-sm text-left text-[#9a9a9a]">Created</p>
            <p class="text-base font-medium text-left text-[#232323]">
              23 Mar 2022
            </p>
          </div>
          <div
            class="flex flex-col justify-start items-start flex-grow relative gap-1"
          >
            <p class="text-sm text-left text-[#9a9a9a]">Dimensions</p>
            <p class="text-base font-medium text-left text-[#232323]">
              1440 x 1080 pixels
            </p>
          </div>
        </div>
        <div class="flex flex-col justify-start items-start relative gap-1">
          <p class="text-sm text-left text-[#9a9a9a]">Model Featured</p>
          <p class="text-base font-medium text-left text-[#232323]">
            Gemma Peach
          </p>
        </div>
      </div>
      <div class="flex flex-col justify-start items-start gap-1.5">
        <div class="flex flex-col justify-start items-start relative gap-1">
          <p class="text-sm text-left text-[#9a9a9a]">Tags</p>
        </div>
        <div class="flex justify-start items-start relative gap-1">
          <div class="w-[90px] h-[30px]">
            <div
              class="w-[90px] h-[30px] absolute left-[-0.5px] top-[-0.5px] bg-[#e0acac]"
            />
            <p
              class="w-[90px] absolute left-0 top-[3px] text-base font-medium text-center text-[#232323]"
            >
              Strap Top
            </p>
          </div>
          <div class="w-[90px] h-[30px]">
            <div
              class="w-[90px] h-[30px] absolute left-[93.5px] top-[-0.5px] bg-[#ace0be]"
            />
            <p
              class="w-[88px] absolute left-24 top-[3px] text-base font-medium text-center text-[#232323]"
            >
              Best
            </p>
          </div>
        </div>
      </div>
    </div>
    <div class="flex justify-center items-center relative gap-3.5">
      <svg
        width="18"
        height="18"
        viewBox="0 0 18 18"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        class="w-[18px] h-[18px] relative"
        preserveAspectRatio="none"
      >
        <path
          d="M11.2509 14.9401L6.36086 10.0501C5.78336 9.47256 5.78336 8.52756 6.36086 7.95006L11.2509 3.06006"
          stroke="#1F206C"
          stroke-width="1.5"
          stroke-miterlimit="10"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
      </svg>
      <div class="flex flex-col justify-start items-center relative w-[483px]">
        <img src={image_14} alt="..." class="h-[645px] object-cover w-full" />
        <div
          class="w-full flex justify-center items-center h-[72px] relative py-4 bg-white"
        >
          <button class="flex justify-start items-center relative gap-2 px-3 py-2">
            <svg
              width="18"
              height="19"
              viewBox="0 0 18 19"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="w-[18px] h-[18px] relative"
              preserveAspectRatio="xMidYMid meet"
            >
              <path
                d="M6.99023 9.26001L8.91023 11.18L10.8302 9.26001"
                stroke="#232323"
                stroke-width="1.5"
                stroke-miterlimit="10"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M8.91016 3.5V11.1275"
                stroke="#232323"
                stroke-width="1.5"
                stroke-miterlimit="10"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M15 9.63501C15 12.95 12.75 15.635 9 15.635C5.25 15.635 3 12.95 3 9.63501"
                stroke="#232323"
                stroke-width="1.5"
                stroke-miterlimit="10"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
            <p class="text-base font-medium text-left text-[#232323]">
              Download
            </p>
          </button>
          <img src={divider_svg} alt="..." />
          <button  class="flex justify-start items-center relative gap-2 px-3 py-2"
          >
            <svg
              width="18"
              height="19"
              viewBox="0 0 18 19"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="w-[18px] h-[18px] relative"
              preserveAspectRatio="xMidYMid meet"
            >
              <path
                d="M3.12779 11.9751L6.52529 15.3726C7.92029 16.7676 10.1853 16.7676 11.5878 15.3726L14.8803 12.0801C16.2753 10.6851 16.2753 8.4201 14.8803 7.0176L11.4753 3.6276C10.7628 2.9151 9.78029 2.5326 8.77529 2.5851L5.02529 2.7651C3.52529 2.8326 2.33279 4.0251 2.25779 5.5176L2.07779 9.2676C2.03279 10.2801 2.41529 11.2626 3.12779 11.9751Z"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M7.125 9.5C8.16053 9.5 9 8.66053 9 7.625C9 6.58947 8.16053 5.75 7.125 5.75C6.08947 5.75 5.25 6.58947 5.25 7.625C5.25 8.66053 6.08947 9.5 7.125 9.5Z"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
              />
            </svg>
            <p class="text-base font-medium text-left text-[#232323]">Tag</p>
          </button>
          <img src={divider_svg} alt="..." />
          <button class="flex justify-start items-center relative gap-2 px-3 py-2">
            <svg
              width="18"
              height="19"
              viewBox="0 0 18 19"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="w-[18px] h-[18px] relative"
              preserveAspectRatio="xMidYMid meet"
            >
              <path
                d="M6.9375 7.2876C8.2725 7.7751 9.7275 7.7751 11.0625 7.2876"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M12.6152 2H5.38523C3.78773 2 2.49023 3.305 2.49023 4.895V15.4625C2.49023 16.8125 3.45773 17.3825 4.64273 16.73L8.30273 14.6975C8.69273 14.48 9.32273 14.48 9.70523 14.6975L13.3652 16.73C14.5502 17.39 15.5177 16.82 15.5177 15.4625V4.895C15.5102 3.305 14.2127 2 12.6152 2Z"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M12.6152 2H5.38523C3.78773 2 2.49023 3.305 2.49023 4.895V15.4625C2.49023 16.8125 3.45773 17.3825 4.64273 16.73L8.30273 14.6975C8.69273 14.48 9.32273 14.48 9.70523 14.6975L13.3652 16.73C14.5502 17.39 15.5177 16.82 15.5177 15.4625V4.895C15.5102 3.305 14.2127 2 12.6152 2Z"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
            <p class="text-base font-medium text-left text-[#232323]">
              Archive
            </p>
          </button>
          <img src={divider_svg} alt="..." />
          <button class="flex justify-start items-center relative gap-2 px-3 py-2">
            <svg
              width="18"
              height="19"
              viewBox="0 0 18 19"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="w-[18px] h-[18px] relative"
              preserveAspectRatio="xMidYMid meet"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M11.25 4.25C11.25 2.59315 12.5931 1.25 14.25 1.25C15.9069 1.25 17.25 2.59315 17.25 4.25C17.25 5.90685 15.9069 7.25 14.25 7.25C13.226 7.25 12.3217 6.73691 11.7804 5.95378L6.57602 8.49079C6.68866 8.80617 6.75 9.14592 6.75 9.5C6.75 9.82963 6.69684 10.1468 6.59862 10.4435L11.7732 13.0567C12.3137 12.2677 13.2214 11.75 14.25 11.75C15.9069 11.75 17.25 13.0931 17.25 14.75C17.25 16.4069 15.9069 17.75 14.25 17.75C12.5931 17.75 11.25 16.4069 11.25 14.75C11.25 14.6587 11.2541 14.5683 11.2621 14.479L5.77885 11.71C5.24477 12.2005 4.53236 12.5 3.75 12.5C2.09315 12.5 0.75 11.1569 0.75 9.5C0.75 7.84315 2.09315 6.5 3.75 6.5C4.50465 6.5 5.19421 6.77864 5.72143 7.23865L11.2636 4.53701C11.2546 4.44255 11.25 4.34681 11.25 4.25ZM15.75 4.25C15.75 3.42157 15.0784 2.75 14.25 2.75C13.4216 2.75 12.75 3.42157 12.75 4.25C12.75 5.07843 13.4216 5.75 14.25 5.75C15.0784 5.75 15.75 5.07843 15.75 4.25ZM15.75 14.75C15.75 13.9216 15.0784 13.25 14.25 13.25C13.4216 13.25 12.75 13.9216 12.75 14.75C12.75 15.5784 13.4216 16.25 14.25 16.25C15.0784 16.25 15.75 15.5784 15.75 14.75ZM3.75 8C4.57843 8 5.25 8.67157 5.25 9.5C5.25 10.3284 4.57843 11 3.75 11C2.92157 11 2.25 10.3284 2.25 9.5C2.25 8.67157 2.92157 8 3.75 8Z"
                fill="#232323"
              />
            </svg>
            <p class="text-base font-medium text-left text-[#232323]">Share</p>
          </button>
          <img src={divider_svg} alt="..." />
          <button class="flex justify-start items-center relative gap-2 px-3 py-2"
          >
            <svg
              width="18"
              height="19"
              viewBox="0 0 18 19"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="w-[18px] h-[18px] relative"
              preserveAspectRatio="xMidYMid meet"
            >
              <path
                d="M15.75 4.98511C13.2525 4.73761 10.74 4.61011 8.235 4.61011C6.75 4.61011 5.265 4.68511 3.78 4.83511L2.25 4.98511"
                stroke="#EB5842"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M6.375 4.2275L6.54 3.245C6.66 2.5325 6.75 2 8.0175 2H9.9825C11.25 2 11.3475 2.5625 11.46 3.2525L11.625 4.2275"
                stroke="#EB5842"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M14.1383 7.35498L13.6508 14.9075C13.5683 16.085 13.5008 17 11.4083 17H6.59328C4.50078 17 4.43328 16.085 4.35078 14.9075L3.86328 7.35498"
                stroke="#EB5842"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M7.74805 12.875H10.2455"
                stroke="#EB5842"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M7.125 9.875H10.875"
                stroke="#EB5842"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
            <p class="text-base font-medium text-left text-[#eb5842]">Delete</p>
          </button>
        </div>
      </div>
      <svg
        width="18"
        height="18"
        viewBox="0 0 18 18"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        class="w-[18px] h-[18px] relative"
        preserveAspectRatio="none"
      >
        <path
          d="M6.68164 14.9401L11.5716 10.0501C12.1491 9.47256 12.1491 8.52756 11.5716 7.95006L6.68164 3.06006"
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

<style>
  p {
    font-family: var(--theme-font-family-base, var(--theme-font-family));
  }
</style>
