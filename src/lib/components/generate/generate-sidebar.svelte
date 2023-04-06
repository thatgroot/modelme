<script lang="ts">
  import { onMount } from "svelte";
  import image_1 from "../../../assets/18.png";
  import RangeSlider from "../range-slider.svelte";

  let file_name: string = "";

  onMount(() => {
    const fileInput = document.getElementById("file");

    fileInput.addEventListener("change", () => {
      //@ts-ignore
      const fileName = fileInput.files[0].name;
      file_name = fileName;
    });

    fileInput.addEventListener("dragover", (e) => {
      e.preventDefault();
    });

    fileInput.addEventListener("drop", (e) => {
      e.preventDefault();
      const fileName = e.dataTransfer.files[0].name;

      file_name = fileName;
    });
  });
</script>

<div
  class="flex flex-col justify-start items-start w-[334px] gap-3 px-8 py-8 bg-white border-t-0 border-r border-b-0 border-l-0 border-[#d9d9d9]"
>
  <div
    class="flex flex-col justify-start items-start self-stretch relative gap-4"
  >
    <input
      type="file"
      id="file"
      class="opacity-0 absolute w-full h-full cursor-pointer z-[999]"
    />
    <div class="flex gap-2 flex-col text-left">
      <span class="text-base font-bold text-left text-[#232323]"
        >#1 Upload
      </span>
      <span class="text-xs text-left text-[#9a9a9a]"
        >Upload your product and company images
      </span>
    </div>
    <div
      class="flex flex-col justify-center items-center self-stretch relative gap-6 px-2.5 py-8 bg-white border-2 border-[#626398] border-dashed"
    >
      <svg
        width="32"
        height="32"
        viewBox="0 0 32 32"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        class="w-8 h-8 relative"
        preserveAspectRatio="xMidYMid meet"
      >
        <path
          d="M27.334 13.5865H23.4806C20.3207 13.5865 17.7473 11.0132 17.7473 7.85317V3.99984C17.7473 3.2665 17.1473 2.6665 16.414 2.6665H10.7607C6.65398 2.6665 3.33398 5.33317 3.33398 10.0932V21.9065C3.33398 26.6665 6.65398 29.3332 10.7607 29.3332H21.2407C25.3473 29.3332 28.6673 26.6665 28.6673 21.9065V14.9198C28.6673 14.1865 28.0673 13.5865 27.334 13.5865ZM15.374 18.0398C15.174 18.2398 14.9207 18.3332 14.6673 18.3332C14.414 18.3332 14.1607 18.2398 13.9607 18.0398L13.0007 17.0798V22.6665C13.0007 23.2132 12.5473 23.6665 12.0007 23.6665C11.454 23.6665 11.0007 23.2132 11.0007 22.6665V17.0798L10.0407 18.0398C9.65398 18.4265 9.01398 18.4265 8.62732 18.0398C8.24065 17.6532 8.24065 17.0132 8.62732 16.6265L11.294 13.9598C11.3873 13.8798 11.4806 13.8132 11.5873 13.7598C11.614 13.7465 11.654 13.7332 11.6807 13.7198C11.7607 13.6932 11.8407 13.6798 11.934 13.6665C11.974 13.6665 12.0007 13.6665 12.0407 13.6665C12.1473 13.6665 12.254 13.6932 12.3607 13.7332C12.374 13.7332 12.374 13.7332 12.3873 13.7332C12.494 13.7732 12.6007 13.8532 12.6807 13.9332C12.694 13.9465 12.7073 13.9465 12.7073 13.9598L15.374 16.6265C15.7606 17.0132 15.7606 17.6532 15.374 18.0398Z"
          fill="#1F206C"
        />
        <path
          d="M23.2409 11.7468C24.5076 11.7602 26.2676 11.7602 27.7742 11.7602C28.5342 11.7602 28.9342 10.8668 28.4009 10.3335C26.4809 8.40015 23.0409 4.92015 21.0676 2.94682C20.5209 2.40015 19.5742 2.77349 19.5742 3.53349V8.18682C19.5742 10.1335 21.2276 11.7468 23.2409 11.7468Z"
          fill="#1F206C"
        />
      </svg>
      <div class="flex flex-col justify-start items-center relative gap-2.5">
        <span class="text-sm text-left text-[#1f206c]">
          <span class="text-sm font-semibold text-left text-[#1f206c]"
            >Upload a file</span
          ><span class="text-sm text-left text-[#1f206c]">
            or drag and drop</span
          >
        </span>
        <span class="text-xs text-left text-[#6c6c6c]">
          PNG, JPG and GIF allowed.
        </span>
      </div>
    </div>
  </div>
  <div
    class="flex flex-col justify-start items-start self-stretch h-[410px] relative gap-3 py-8"
  >
    <span class="text-left">
      <span class="text-base font-bold text-left text-[#232323]"
        >#2 Select
      </span><br /><span class="text-xs text-left text-[#9a9a9a]"
        >Select the model you wish to feature</span
      >
    </span>
    <div class="flex flex-col gap-1 items-center w-full">
      <img src={image_1} alt="..." class=" h-[296px] object-cover w-full" />
      <div class="flex justify-center items-center w-[180px] ">
        <div
          class="flex justify-center items-center self-stretch flex-grow relative py-3 bg-white"
        >
          <svg
            width="19"
            height="18"
            viewBox="0 0 19 18"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            class="w-[18px] h-[18px] relative"
            preserveAspectRatio="none"
          >
            <path
              d="M11.7509 14.9401L6.86086 10.0501C6.28336 9.47256 6.28336 8.52756 6.86086 7.95006L11.7509 3.06006"
              stroke="#1F206C"
              stroke-width="1.5"
              stroke-miterlimit="10"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </svg>
        </div>
        <span class="w-[179px] text-base text-center text-[#232323]"
          >Gemma Peach
        </span>
        <div
          class="flex justify-center items-center self-stretch flex-grow relative py-3 bg-white"
        >
          <svg
            width="19"
            height="18"
            viewBox="0 0 19 18"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            class="w-[18px] h-[18px] relative"
            preserveAspectRatio="none"
          >
            <path
              d="M7.18164 14.9401L12.0716 10.0501C12.6491 9.47256 12.6491 8.52756 12.0716 7.95006L7.18164 3.06006"
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
  <div class="flex flex-col justify-start items-start gap-3 py-8 mt-4">
    <div class="flex flex-col justify-start items-start relative gap-2">
      <div class="flex justify-between items-center w-[270px] relative">
        <span class="text-left">
          <span class="text-base font-bold text-left text-[#232323]"
            >#3 Generate</span
          ><br /><span class="text-xs text-left text-[#9a9a9a]"
            >Number of generated images per uploaded image</span
          >
        </span>
      </div>
      <RangeSlider min={0} max={12} />
    </div>
  </div>
  <div class="flex flex-col justify-start items-start relative gap-3 py-8">
    <button
      class="flex justify-center items-center w-[270px] relative gap-2 p-3 bg-[#1f206c]"
    >
      <span class="text-sm font-medium text-center text-white">
        Generate 4 images
      </span>
    </button>
    <span class="text-xs text-center text-[#9a9a9a]">
      This generation is worth 4 credits
    </span>
  </div>
</div>
