<div class="flex  items-center justify-between gap-4">
  <div
    class="flex flex-col justify-center items-center flex-grow-0 flex-shrink-0 w-[366px] relative p-4 bg-white border border-[#1f206c]"
  >
    <p
      class="self-stretch flex-grow-0 flex-shrink-0 w-[334px] text-lg font-medium text-left text-[#9a9a9a]"
    >
      Search...
    </p>
  </div>
  <div class="flex flex-grow justify-between items-center">
    <div
      class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-2"
    >
      <svg
        width="24"
        height="25"
        viewBox="0 0 24 25"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        class="flex-grow-0 flex-shrink-0 w-6 h-6 relative"
        preserveAspectRatio="xMidYMid meet"
      >
        <path
          d="M9.3 21.5H14.7C19.2 21.5 21 19.7 21 15.2V9.8C21 5.3 19.2 3.5 14.7 3.5H9.3C4.8 3.5 3 5.3 3 9.8V15.2C3 19.7 4.8 21.5 9.3 21.5Z"
          stroke="#9A9A9A"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
      </svg>
      <p
        class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-[#9a9a9a]"
      >
        Select all
      </p>
    </div>
    <div
      class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-4"
    >
      <div id="sort" class="relative group">
        <div class="flex gap-4 items-center relative">
          <p
            class="flex-grow-0 flex-shrink-0 text-base text-left text-[#9a9a9a]"
          >
            Sort by:
          </p>
          <div
            class="flex justify-center items-center flex-grow-0 flex-shrink-0 relative gap-2 p-3 border border-[#1f206c]"
          >
            <svg
              width="18"
              height="19"
              viewBox="0 0 18 19"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="flex-grow-0 flex-shrink-0 w-[18px] h-[18px] relative"
              preserveAspectRatio="none"
            >
              <path
                d="M13.5523 7.6775L8.99977 3.125L4.44727 7.6775"
                stroke="#232323"
                stroke-width="1.5"
                stroke-miterlimit="10"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M9 15.8749V3.25244"
                stroke="#232323"
                stroke-width="1.5"
                stroke-miterlimit="10"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
            <p
              class="flex-grow-0 flex-shrink-0 text-sm font-medium text-center text-[#232323]"
            >
              Folders
            </p>
            <svg
              width="18"
              height="19"
              viewBox="0 0 18 19"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="flex-grow-0 flex-shrink-0 w-[18px] h-[18px] relative"
              preserveAspectRatio="none"
            >
              <path
                d="M14.9405 7.2124L10.0505 12.1024C9.47305 12.6799 8.52805 12.6799 7.95055 12.1024L3.06055 7.2124"
                stroke="#232323"
                stroke-width="1.5"
                stroke-miterlimit="10"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
        </div>
        <div
          class="hidden group-hover:flex flex-col justify-start items-start w-[293px] absolute right-0 z-[999] my-1 gap-4 p-4 bg-white border border-[#d9d9d9]"
          style="box-shadow: 4px 4px 44px 0 rgba(0,0,0,0.08);"
        >
          <p
            class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-[#232323]"
          >
            Sort by
          </p>
          {#each ["Kind", "Date Created", "Name"] as filter}
            <div
              class="flex justify-start items-center self-stretch flex-grow-0 flex-shrink-0 relative gap-2 py-2"
            >
              <div
                class="flex justify-start items-start flex-grow-0 flex-shrink-0 relative gap-2.5 rounded-[100px]"
              >
                <svg
                  width="20"
                  height="20"
                  viewBox="0 0 20 20"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                  class="flex-grow-0 flex-shrink-0"
                  preserveAspectRatio="xMidYMid meet"
                >
                  <circle
                    cx="10"
                    cy="10"
                    r="8.5"
                    stroke="#D9D9D9"
                    stroke-width="3"
                  />
                </svg>
              </div>
              <p
                class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-[#232323]"
              >
                {filter}
              </p>
            </div>
          {/each}
        </div>
      </div>

      <div id="filter" class="relative group">
        <div class="flex gap-4 items-center relative">
          <p
            class="flex-grow-0 flex-shrink-0 text-base text-left text-[#9a9a9a]"
          >
            Filter by:
          </p>
          <div
            class="flex justify-center items-center flex-grow-0 flex-shrink-0 relative gap-2 p-3 border border-[#1f206c]"
          >
            <svg
              width="18"
              height="19"
              viewBox="0 0 18 19"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="flex-grow-0 flex-shrink-0 w-[18px] h-[18px] relative"
              preserveAspectRatio="none"
            >
              <path
                d="M13.5523 7.6775L8.99977 3.125L4.44727 7.6775"
                stroke="#232323"
                stroke-width="1.5"
                stroke-miterlimit="10"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M9 15.8749V3.25244"
                stroke="#232323"
                stroke-width="1.5"
                stroke-miterlimit="10"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
            <p
              class="flex-grow-0 flex-shrink-0 text-sm font-medium text-center text-[#232323]"
            >
              Tag
            </p>
            <svg
              width="18"
              height="19"
              viewBox="0 0 18 19"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="flex-grow-0 flex-shrink-0 w-[18px] h-[18px] relative"
              preserveAspectRatio="none"
            >
              <path
                d="M14.9405 7.2124L10.0505 12.1024C9.47305 12.6799 8.52805 12.6799 7.95055 12.1024L3.06055 7.2124"
                stroke="#232323"
                stroke-width="1.5"
                stroke-miterlimit="10"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
        </div>
        <div
          class="hidden group-hover:flex flex-col justify-start items-start w-[293px] absolute right-0 z-[999] my-1 gap-4 p-4 bg-white border border-[#d9d9d9]"
          style="box-shadow: 4px 4px 44px 0 rgba(0,0,0,0.08);"
        >
          <p
            class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-[#232323]"
          >
            Filter by
          </p>
          {#each ["Tag", "License"] as filter}
            <div
              class="flex justify-start items-center self-stretch flex-grow-0 flex-shrink-0 relative gap-2 py-2"
            >
              <div
                class="flex justify-start items-start flex-grow-0 flex-shrink-0 relative gap-2.5 rounded-[100px]"
              >
                <svg
                  width="20"
                  height="20"
                  viewBox="0 0 20 20"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                  class="flex-grow-0 flex-shrink-0"
                  preserveAspectRatio="xMidYMid meet"
                >
                  <circle
                    cx="10"
                    cy="10"
                    r="8.5"
                    stroke="#D9D9D9"
                    stroke-width="3"
                  />
                </svg>
              </div>
              <p
                class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-[#232323]"
              >
                {filter}
              </p>
            </div>
          {/each}
        </div>
      </div>

      <div id="view" class="relative group">
        <div class="flex gap-4 items-center relative">
          <div
            class="flex justify-center items-center flex-grow-0 flex-shrink-0 relative gap-2 p-3 border border-[#1f206c]"
          >
            <p
              class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-[#9a9a9a]"
            >
              View:
            </p>
            <svg
              width="18"
              height="19"
              viewBox="0 0 18 19"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="flex-grow-0 flex-shrink-0 w-[18px] h-[18px] relative"
              preserveAspectRatio="xMidYMid meet"
            >
              <path
                d="M16.5 6.89V3.485C16.5 2.4275 16.02 2 14.8275 2H11.7975C10.605 2 10.125 2.4275 10.125 3.485V6.8825C10.125 7.9475 10.605 8.3675 11.7975 8.3675H14.8275C16.02 8.375 16.5 7.9475 16.5 6.89Z"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M16.5 15.3275V12.2975C16.5 11.105 16.02 10.625 14.8275 10.625H11.7975C10.605 10.625 10.125 11.105 10.125 12.2975V15.3275C10.125 16.52 10.605 17 11.7975 17H14.8275C16.02 17 16.5 16.52 16.5 15.3275Z"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M7.875 6.89V3.485C7.875 2.4275 7.395 2 6.2025 2H3.1725C1.98 2 1.5 2.4275 1.5 3.485V6.8825C1.5 7.9475 1.98 8.3675 3.1725 8.3675H6.2025C7.395 8.375 7.875 7.9475 7.875 6.89Z"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M7.875 15.3275V12.2975C7.875 11.105 7.395 10.625 6.2025 10.625H3.1725C1.98 10.625 1.5 11.105 1.5 12.2975V15.3275C1.5 16.52 1.98 17 3.1725 17H6.2025C7.395 17 7.875 16.52 7.875 15.3275Z"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
            <p
              class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-[#232323]"
            >
              Grid
            </p>
            <svg
              width="16"
              height="17"
              viewBox="0 0 16 17"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="flex-grow-0 flex-shrink-0 w-4 h-4 relative"
              preserveAspectRatio="xMidYMid meet"
            >
              <path
                d="M13.2807 6.4668L8.93404 10.8135C8.4207 11.3268 7.5807 11.3268 7.06737 10.8135L2.7207 6.4668"
                stroke="#9A9A9A"
                stroke-width="1.5"
                stroke-miterlimit="10"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
        </div>

        <div
          class="hidden group-hover:flex absolute right-0 flex-col justify-start items-start w-[293px] z-[999] my-1 gap-4 p-4 bg-white border border-[#d9d9d9]"
          style="box-shadow: 4px 4px 44px 0 rgba(0,0,0,0.08);"
        >
          <div
            class="flex relative flex-shrink-0 flex-grow-0 items-center justify-between self-stretch"
          >
            <p
              class="flex-shrink-0 flex-grow-0 text-left text-base font-medium text-[#232323]"
            >
              View
            </p>
            <svg
              width="18"
              height="18"
              viewBox="0 0 18 18"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="relative h-[18px] w-[18px] flex-shrink-0 flex-grow-0"
              preserveAspectRatio="xMidYMid meet"
            >
              <path
                d="M3.75 3.75L14.2493 14.2493"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M3.75071 14.2493L14.25 3.75"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
          <div
            class="flex relative flex-shrink-0 flex-grow-0 items-center justify-start gap-2 self-stretch py-2"
          >
            <div
              class="flex relative flex-shrink-0 flex-grow-0 items-start justify-start gap-2.5 rounded-[100px]"
            >
              <svg
                width="20"
                height="20"
                viewBox="0 0 20 20"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="flex-shrink-0 flex-grow-0"
                preserveAspectRatio="xMidYMid meet"
              >
                <circle
                  cx="10"
                  cy="10"
                  r="8.5"
                  stroke="#D9D9D9"
                  stroke-width="3"
                />
              </svg>
            </div>
            <svg
              width="18"
              height="18"
              viewBox="0 0 18 18"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="relative h-[18px] w-[18px] flex-shrink-0 flex-grow-0"
              preserveAspectRatio="xMidYMid meet"
            >
              <path
                d="M16.5 6.39V2.985C16.5 1.9275 16.02 1.5 14.8275 1.5H11.7975C10.605 1.5 10.125 1.9275 10.125 2.985V6.3825C10.125 7.4475 10.605 7.8675 11.7975 7.8675H14.8275C16.02 7.875 16.5 7.4475 16.5 6.39Z"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M16.5 14.8275V11.7975C16.5 10.605 16.02 10.125 14.8275 10.125H11.7975C10.605 10.125 10.125 10.605 10.125 11.7975V14.8275C10.125 16.02 10.605 16.5 11.7975 16.5H14.8275C16.02 16.5 16.5 16.02 16.5 14.8275Z"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M7.875 6.39V2.985C7.875 1.9275 7.395 1.5 6.2025 1.5H3.1725C1.98 1.5 1.5 1.9275 1.5 2.985V6.3825C1.5 7.4475 1.98 7.8675 3.1725 7.8675H6.2025C7.395 7.875 7.875 7.4475 7.875 6.39Z"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M7.875 14.8275V11.7975C7.875 10.605 7.395 10.125 6.2025 10.125H3.1725C1.98 10.125 1.5 10.605 1.5 11.7975V14.8275C1.5 16.02 1.98 16.5 3.1725 16.5H6.2025C7.395 16.5 7.875 16.02 7.875 14.8275Z"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
            <p
              class="flex-shrink-0 flex-grow-0 text-left text-base font-medium text-[#232323]"
            >
              Grid
            </p>
          </div>
          <div
            class="flex relative flex-shrink-0 flex-grow-0 items-center justify-start gap-2 self-stretch py-2"
          >
            <div
              class="flex relative flex-shrink-0 flex-grow-0 items-start justify-start gap-2.5 rounded-[100px]"
            >
              <svg
                width="20"
                height="20"
                viewBox="0 0 20 20"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="flex-shrink-0 flex-grow-0"
                preserveAspectRatio="xMidYMid meet"
              >
                <circle
                  cx="10"
                  cy="10"
                  r="8.5"
                  stroke="#D9D9D9"
                  stroke-width="3"
                />
              </svg>
            </div>
            <svg
              width="18"
              height="18"
              viewBox="0 0 18 18"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="relative h-[18px] w-[18px] flex-shrink-0 flex-grow-0"
              preserveAspectRatio="xMidYMid meet"
            >
              <path
                d="M2.25 3.375H15.75"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M2.25 7.125H15.75"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M2.25 10.875H15.75"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M2.25 14.625H15.75"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
            <p
              class="flex-shrink-0 flex-grow-0 text-left text-base font-medium text-[#232323]"
            >
              Lists
            </p>
          </div>
          <div
            class="flex relative flex-shrink-0 flex-grow-0 items-center justify-start gap-2 self-stretch py-2"
          >
            <div
              class="flex relative flex-shrink-0 flex-grow-0 items-start justify-start gap-2.5 rounded-[100px] border-2 border-[#1f206c] p-1"
            >
              <svg
                width="12"
                height="12"
                viewBox="0 0 12 12"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="flex-shrink-0 flex-grow-0"
                preserveAspectRatio="xMidYMid meet"
              >
                <circle cx="6" cy="6" r="6" fill="#1F206C" />
              </svg>
            </div>
            <svg
              width="18"
              height="18"
              viewBox="0 0 18 18"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="relative h-[18px] w-[18px] flex-shrink-0 flex-grow-0"
              preserveAspectRatio="xMidYMid meet"
            >
              <path
                d="M14.925 7.875L3.075 7.875C1.95 7.875 1.5 7.395 1.5 6.2025L1.5 3.1725C1.5 1.98 1.95 1.5 3.075 1.5L14.925 1.5C16.05 1.5 16.5 1.98 16.5 3.1725V6.2025C16.5 7.395 16.05 7.875 14.925 7.875Z"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M6.39 16.5H2.985C1.9275 16.5 1.5 16.02 1.5 14.8275L1.5 11.7975C1.5 10.605 1.9275 10.125 2.985 10.125H6.3825C7.4475 10.125 7.8675 10.605 7.8675 11.7975L7.8675 14.8275C7.875 16.02 7.4475 16.5 6.39 16.5Z"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M14.8275 16.5H11.7975C10.605 16.5 10.125 16.02 10.125 14.8275V11.7975C10.125 10.605 10.605 10.125 11.7975 10.125H14.8275C16.02 10.125 16.5 10.605 16.5 11.7975V14.8275C16.5 16.02 16.02 16.5 14.8275 16.5Z"
                stroke="#232323"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
            <p
              class="flex-shrink-0 flex-grow-0 text-left text-base font-medium text-[#232323]"
            >
              Column (Images)
            </p>
          </div>
          <div class="relative w-full ">
            <div class="bg-red relative  py-4">

              <input type="range" name="" id="" class="w-full accent-[#000000] h-[3px]" />

              <p
                class="absolute left-4 top-10 text-left text-base font-medium text-[#232323]"
              >
                0
              </p>
              <p
                class="absolute right-4 top-10 text-left text-base font-medium text-[#232323]"
              >
                12
              </p>
            </div>
            <div
              class="flex absolute left-0 right-0 -top-5 mx-auto w-fit flex-col items-start justify-start gap-2.5 bg-[#232323] px-3 py-1"
            >
              <p
                class="flex-shrink-0 flex-grow-0 text-left text-base font-medium text-white"
              >
                8
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
