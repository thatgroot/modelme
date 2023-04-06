<script lang="ts">
  import image_2 from "../../../assets/32.png";
  import image_5 from "../../../assets/33.png";
  import image_3 from "../../../assets/34.png";
  import image_4 from "../../../assets/35.png";
  import image_1 from "../../../assets/36.png";
  import Badge from "../badge.svelte";
  import CardOverlay from "../card-overlay.svelte";
  import Revolver from "../revolver.svelte";
</script>

<div
  id="gallery"
  class="flex flex-col justify-start items-center flex-grow-0 flex-shrink-0 overflow-hidden gap-16 pt-9 bg-white border-t-0 border-r-0 border-b border-l-0 border-[#232323]/[0.16]"
>
  <div
    class="flex flex-col justify-start items-center flex-grow-0 flex-shrink-0 gap-6"
  >
    <div
      class="flex flex-col justify-center items-end flex-grow-0 flex-shrink-0 relative gap-3"
    >
      <div
        class="flex justify-center items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-2.5 p-2.5"
      >
        <span
          class="flex-grow-0 flex-shrink-0 text-lg font-semibold text-left text-[#1f206c]"
        >
          MODELME GALLERY
        </span>
      </div>
      <div
        class="flex justify-end items-center self-stretch flex-grow-0 flex-shrink-0 relative gap-[18px]"
      >
        <p
          class="flex-grow-0 flex-shrink-0 text-[58px] text-left text-neutral-900"
        >
          CREATED CONTENT
        </p>
        <div class="flex-grow-0 flex-shrink-0 w-[202px] h-[41px]">
          <svg
            width="203"
            height="42"
            viewBox="0 0 203 42"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            class="absolute left-[403.5px] top-3.5"
            preserveAspectRatio="none"
          >
            <path
              d="M0.5 0.64917H178.5L160.5 41.6492H0.5V0.64917Z"
              fill="#1F206C"
            />
            <path
              d="M0.5 0.64917H178.5L160.5 41.6492H0.5V0.64917Z"
              fill="#1F206C"
            />
            <path
              d="M184.5 0.64917H190.5L172.5 41.6492H166.5L184.5 0.64917Z"
              fill="#1F206C"
            />
            <path
              d="M196.5 0.64917H202.5L184.5 41.6492H178.5L196.5 0.64917Z"
              fill="#1F206C"
            />
          </svg>
          <span
            class="absolute left-[412px] top-[23px] text-lg font-bold text-left text-white"
          >
            Men coming soon
          </span>
        </div>
      </div>
      <span
        class="flex-grow-0 flex-shrink-0 w-[606px] text-lg text-center text-[#757575]"
      >
        Content creators generate sustainable and diverse imagery to advertise
        their company and products. Produce on-model fashion imagery and more.
      </span>
    </div>
    <div
      class="flex justify-start items-start flex-grow-0 flex-shrink-0 w-[1227px] gap-5"
    >
      <div
        class="flex flex-col justify-start items-center self-stretch flex-grow gap-5"
      >
        <div
          class="flex flex-col justify-start items-start w-[505px] relative gap-2.5 p-2.5  group overflow-hidden"
        >
          <img
            src={image_1}
            alt="..."
            style="background: linear-gradient(134.88deg, #ececec -9.28%, rgba(236,236,236,0) 109.69%);"
          />

          <div
            class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 absolute left-10 top-10 gap-3"
          >
            <span
              class="flex-grow-0 flex-shrink-0 text-[22px] font-semibold text-left text-white"
            >
              Diversity in seconds
            </span>
            <span
              class="flex-grow-0 flex-shrink-0 text-lg text-left text-[#fffefe]"
            >
              Home Decor - eComm
            </span>
            <span
              class="flex-grow-0 flex-shrink-0 opacity-50 text-sm text-left text-[#fffbfb]"
            >
              by Stomata
            </span>
          </div>
          <div class="absolute right-4 bottom-6 hidden group-hover:block">
            <Badge lable="Uploaded" />
          </div>
        </div>
        <div
          class="flex justify-start items-start self-stretch flex-grow-0 flex-shrink-0 h-[334px] relative group overflow-hidden"
          style="background: linear-gradient(204.3deg, #cfc5ba 53.05%, rgba(207,197,186,0.58) 83.73%, rgba(207,197,186,0) 89.99%);"
        >
          <img
            src={image_2}
            alt="..."
            class="self-stretch flex-grow-0 flex-shrink-0 w-[290px] object-cover"
          />
          <div
            class="flex flex-col justify-start items-end flex-grow-0 flex-shrink-0 w-[505px] absolute left-[0.5px] top-[-0.15px] gap-2.5 pr-10 pt-10 pb-2.5"
          >
            <div
              class="flex flex-col justify-start items-end flex-grow-0 flex-shrink-0 relative gap-[5px]"
            >
              <span
                class="flex-grow-0 flex-shrink-0 text-[22px] font-semibold text-left text-neutral-900"
              >
                Royalty free
              </span>
              <span
                class="flex-grow-0 flex-shrink-0 text-lg text-left text-neutral-900"
              >
                Jewellery - Social Media
              </span>
              <span
                class="flex-grow-0 flex-shrink-0 opacity-50 text-sm text-left text-neutral-900"
              >
                by Juno-Uno
              </span>
            </div>
          </div>
          <div class="absolute right-4 bottom-6 hidden group-hover:block">
            <Badge lable="Uploaded" />
          </div>
        </div>
      </div>
      <div
        class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 gap-5"
      >
        <div
          class="flex justify-start items-start self-stretch flex-grow gap-5"
        >
          <div
            class="flex flex-col justify-start items-start self-stretch flex-grow relative group overflow-hidden bg-neutral-100"
          >
            <div
              class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 relative gap-2 pl-6 pt-6"
            >
              <span
                class="flex-grow-0 flex-shrink-0 text-[22px] font-semibold text-left text-neutral-900"
              >
                Personalised imagery
              </span>
              <span
                class="flex-grow-0 flex-shrink-0 text-lg text-left text-neutral-900"
              >
                Apparel - eComm
              </span>
              <span
                class="flex-grow-0 flex-shrink-0 opacity-50 text-sm text-left text-neutral-900"
              >
                by Stomata
              </span>
            </div>
            <img
              src={image_3}
              alt="..."
              class="flex-grow w-[344px] object-cover"
            />
            <div class="absolute right-4 bottom-6 hidden group-hover:block">
              <Badge lable="Uploaded" />
            </div>
          </div>
          <div
            class="flex flex-col justify-start items-center self-stretch flex-grow-0 flex-shrink-0 w-[341px] group relative overflow-hidden"
            style="background: linear-gradient(215.55deg, #b7b1aa -14.4%, rgba(236,236,236,0) 105.08%);"
          >
            <img
              src={image_4}
              alt="..."
              class="flex-grow w-[537px] object-cover absolute bottom-0"
            />
            <div
              class="flex flex-col justify-start items-end flex-grow-0 flex-shrink-0 absolute left-[156px] top-10 gap-2"
            >
              <span
                class="flex-grow-0 flex-shrink-0 text-[22px] font-semibold text-right text-neutral-900"
              >
                Easy to edit
              </span>
              <span
                class="flex-grow-0 flex-shrink-0 text-lg text-right text-black"
              >
                Apparel - eComm
              </span>
              <span
                class="flex-grow-0 flex-shrink-0 opacity-50 text-sm text-right text-neutral-900"
              >
                by Luke
              </span>
            </div>
            <div class="absolute right-4 bottom-6 hidden group-hover:block">
              <Badge lable="Uploaded" />
            </div>
          </div>
        </div>
        <div

          class="flex flex-col justify-start items-start self-stretch flex-grow-0 flex-shrink-0 h-[635px] relative group overflow-hidden"
          style="background: linear-gradient(134.88deg, #ececec -9.28%, rgba(236,236,236,0) 109.69%);"
        >
          <img
            src={image_5}
            alt="..."
            class="flex-grow w-[702px] object-cover"
          />
          <div
            class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 absolute left-10 top-10 gap-2"
          >
            <span
              class="flex-grow-0 flex-shrink-0 text-[22px] font-semibold text-left text-white"
            >
              High resolution
            </span>
            <span class="flex-grow-0 flex-shrink-0 text-lg text-left text-white">
              Art Project
            </span>
            <span
              class="flex-grow-0 flex-shrink-0 opacity-50 text-sm text-left text-white"
            >
              by Luperpla
            </span>
          </div>
          <div class="absolute right-4 bottom-6 hidden group-hover:block">
            <Badge lable="Uploaded" />
          </div>
        </div>
      </div>
    </div>
  </div>
  <Revolver />
</div>
