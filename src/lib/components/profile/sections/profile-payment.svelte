<script lang="ts">
  import Modal from "../../modal.svelte";

  let show_modal: boolean = false;
</script>

<div class="flex justify-start items-start gap-[17px]">
  <div
    class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 w-[436px] gap-6 p-6 bg-white"
  >
    <div
      class="flex justify-start items-center self-stretch flex-grow-0 flex-shrink-0 relative gap-4 p-4 bg-[#1f206c]"
    >
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
          d="M12 12.5C14.7614 12.5 17 10.2614 17 7.5C17 4.73858 14.7614 2.5 12 2.5C9.23858 2.5 7 4.73858 7 7.5C7 10.2614 9.23858 12.5 12 12.5Z"
          fill="white"
        />
        <path
          d="M12.0002 15C6.99016 15 2.91016 18.36 2.91016 22.5C2.91016 22.78 3.13016 23 3.41016 23H20.5902C20.8702 23 21.0902 22.78 21.0902 22.5C21.0902 18.36 17.0102 15 12.0002 15Z"
          fill="white"
        />
      </svg>
      <p
        class="flex-grow-0 flex-shrink-0 text-lg font-medium text-left text-white"
      >
        General
      </p>
    </div>
    <div
      class="flex justify-start items-center self-stretch flex-grow-0 flex-shrink-0 relative gap-4 p-4 bg-white"
    >
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
          d="M17.4395 15.12L19.9995 12.56L17.4395 10"
          stroke="#EB5842"
          stroke-width="1.5"
          stroke-miterlimit="10"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M9.75977 12.56H19.9298"
          stroke="#EB5842"
          stroke-width="1.5"
          stroke-miterlimit="10"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M11.7598 20.5C7.33977 20.5 3.75977 17.5 3.75977 12.5C3.75977 7.5 7.33977 4.5 11.7598 4.5"
          stroke="#EB5842"
          stroke-width="1.5"
          stroke-miterlimit="10"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
      </svg>
      <p
        class="flex-grow-0 flex-shrink-0 text-lg font-medium text-left text-[#eb5842]"
      >
        Logout
      </p>
    </div>
  </div>
  <div
    class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 gap-8"
  >
    <div
      class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 w-[888px] relative gap-8 p-8 bg-white"
    >
      <div
        class="flex flex-col justify-start items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-4"
      >
        <p
          class="flex-grow-0 flex-shrink-0 text-lg font-semibold text-left text-[#232323]"
        >
          Account Information
        </p>
        <div
          class="flex flex-col justify-start items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-2"
        >
          <p
            class="flex-grow-0 flex-shrink-0 w-[327px] text-sm font-semibold text-left text-[#232323]"
          >
            Email
          </p>
          <div
            class="flex flex-col justify-center items-center self-stretch flex-grow-0 flex-shrink-0 relative p-4 bg-[#e9e9f0] border border-[#1f206c]"
          >
            <p
              class="self-stretch flex-grow-0 flex-shrink-0 w-[792px] text-lg font-medium text-left text-[#1f206c]"
            >
              ganteng@mail.com
            </p>
          </div>
        </div>
        <div
          class="flex flex-col justify-start items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-2"
        >
          <p
            class="flex-grow-0 flex-shrink-0 w-[327px] text-sm font-semibold text-left text-[#232323]"
          >
            Password
          </p>
          <div
            class="flex flex-col justify-center items-center self-stretch flex-grow-0 flex-shrink-0 p-4 bg-[#e9e9f0] border border-[#1f206c]"
          >
            <div
              class="flex justify-start items-center self-stretch flex-grow-0 flex-shrink-0 h-[27px] relative gap-2"
            >
              <svg
                width="8"
                height="9"
                viewBox="0 0 8 9"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="flex-grow-0 flex-shrink-0"
                preserveAspectRatio="xMidYMid meet"
              >
                <circle cx="4" cy="4.5" r="4" fill="#232323" /></svg
              ><svg
                width="8"
                height="9"
                viewBox="0 0 8 9"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="flex-grow-0 flex-shrink-0"
                preserveAspectRatio="xMidYMid meet"
              >
                <circle cx="4" cy="4.5" r="4" fill="#232323" /></svg
              ><svg
                width="8"
                height="9"
                viewBox="0 0 8 9"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="flex-grow-0 flex-shrink-0"
                preserveAspectRatio="xMidYMid meet"
              >
                <circle cx="4" cy="4.5" r="4" fill="#232323" /></svg
              ><svg
                width="8"
                height="9"
                viewBox="0 0 8 9"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="flex-grow-0 flex-shrink-0"
                preserveAspectRatio="xMidYMid meet"
              >
                <circle cx="4" cy="4.5" r="4" fill="#232323" /></svg
              ><svg
                width="8"
                height="9"
                viewBox="0 0 8 9"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="flex-grow-0 flex-shrink-0"
                preserveAspectRatio="xMidYMid meet"
              >
                <circle cx="4" cy="4.5" r="4" fill="#232323" /></svg
              ><svg
                width="8"
                height="9"
                viewBox="0 0 8 9"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="flex-grow-0 flex-shrink-0"
                preserveAspectRatio="xMidYMid meet"
              >
                <circle cx="4" cy="4.5" r="4" fill="#232323" /></svg
              ><svg
                width="8"
                height="9"
                viewBox="0 0 8 9"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="flex-grow-0 flex-shrink-0"
                preserveAspectRatio="xMidYMid meet"
              >
                <circle cx="4" cy="4.5" r="4" fill="#232323" /></svg
              ><svg
                width="8"
                height="9"
                viewBox="0 0 8 9"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="flex-grow-0 flex-shrink-0"
                preserveAspectRatio="xMidYMid meet"
              >
                <circle cx="4" cy="4.5" r="4" fill="#232323" />
              </svg>
            </div>
          </div>
        </div>
      </div>
      <div
        class="flex flex-col justify-start items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-4"
      >
        <p
          class="flex-grow-0 flex-shrink-0 text-lg font-semibold text-left text-[#232323]"
        >
          Subscriptions
        </p>
        <div
          class="flex justify-start items-start self-stretch flex-grow-0 flex-shrink-0 gap-2"
        >
          <div
            class="flex flex-col justify-start items-center flex-grow relative bg-[#626398]"
          >
            <div
              class="flex flex-col justify-start items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-2 p-4"
            >
              <div
                class="flex justify-between items-center self-stretch flex-grow-0 flex-shrink-0 relative"
              >
                <p
                  class="flex-grow-0 flex-shrink-0 text-sm font-semibold text-left text-white"
                >
                  Subscription Title
                </p>
                <svg
                  width="19"
                  height="19"
                  viewBox="0 0 19 19"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                  class="flex-grow-0 flex-shrink-0 w-[18px] h-[18px] relative"
                  preserveAspectRatio="xMidYMid meet"
                >
                  <path
                    d="M9.33398 2C5.20148 2 1.83398 5.3675 1.83398 9.5C1.83398 13.6325 5.20148 17 9.33398 17C13.4665 17 16.834 13.6325 16.834 9.5C16.834 5.3675 13.4665 2 9.33398 2ZM12.919 7.775L8.66648 12.0275C8.56148 12.1325 8.41898 12.1925 8.26898 12.1925C8.11898 12.1925 7.97648 12.1325 7.87148 12.0275L5.74898 9.905C5.53148 9.6875 5.53148 9.3275 5.74898 9.11C5.96648 8.8925 6.32648 8.8925 6.54398 9.11L8.26898 10.835L12.124 6.98C12.3415 6.7625 12.7015 6.7625 12.919 6.98C13.1365 7.1975 13.1365 7.55 12.919 7.775Z"
                    fill="white"
                  />
                </svg>
              </div>
              <p
                class="flex-grow-0 flex-shrink-0 w-[215px] text-xs text-left text-[#a5a6c4]"
              >
                Lorem ipsum dolor sit amet consectetur. A in aliquet a ac
                volutpat.
              </p>
            </div>
            <svg
              width="248"
              height="2"
              viewBox="0 0 248 2"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="flex-grow-0 flex-shrink-0"
              preserveAspectRatio="none"
            >
              <path d="M0.166016 1H247.166" stroke="#D9D9D9" />
            </svg>
            <div
              class="flex justify-start items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-2.5 p-4 bg-[#f9f9f9]"
            >
              <p
                class="flex-grow w-[113.67px] text-xs text-left text-[#9a9a9a]"
              >
                Learn more
              </p>
              <p
                class="flex-grow w-[113.67px] text-xs text-right text-[#232323]"
              >
                <span
                  class="flex-grow w-[113.67px] text-xs font-semibold text-right text-[#232323]"
                  >$10.99</span
                ><span
                  class="flex-grow w-[113.67px] text-xs text-right text-[#232323]"
                  >/month</span
                >
              </p>
            </div>
          </div>
          <div
            class="flex flex-col justify-start items-center flex-grow relative bg-[#4f4f4f]"
          >
            <div
              class="flex flex-col justify-start items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-2 p-4"
            >
              <div
                class="flex justify-between items-center self-stretch flex-grow-0 flex-shrink-0 relative"
              >
                <p
                  class="flex-grow-0 flex-shrink-0 text-sm font-semibold text-left text-white"
                >
                  Subscription Title
                </p>
                <svg
                  width="19"
                  height="19"
                  viewBox="0 0 19 19"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                  class="flex-grow-0 flex-shrink-0"
                  preserveAspectRatio="xMidYMid meet"
                >
                  <circle cx="9.66797" cy="9.5" r="8.5" stroke="white" />
                </svg>
              </div>
              <p
                class="flex-grow-0 flex-shrink-0 w-[215px] text-xs text-left text-[#9a9a9a]"
              >
                Lorem ipsum dolor sit amet consectetur. A in aliquet a ac
                volutpat.
              </p>
            </div>
            <svg
              width="248"
              height="2"
              viewBox="0 0 248 2"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="flex-grow-0 flex-shrink-0"
              preserveAspectRatio="none"
            >
              <path d="M0.5 1H247.5" stroke="#D9D9D9" />
            </svg>
            <div
              class="flex justify-start items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-2.5 p-4 bg-[#f9f9f9]"
            >
              <p
                class="flex-grow w-[113.67px] text-xs text-left text-[#9a9a9a]"
              >
                Learn more
              </p>
              <p
                class="flex-grow w-[113.67px] text-xs text-right text-[#232323]"
              >
                <span
                  class="flex-grow w-[113.67px] text-xs font-semibold text-right text-[#232323]"
                  >$10.99</span
                ><span
                  class="flex-grow w-[113.67px] text-xs text-right text-[#232323]"
                  >/month</span
                >
              </p>
            </div>
          </div>
          <div
            class="flex flex-col justify-start items-center flex-grow relative bg-[#339dff]"
          >
            <div
              class="flex flex-col justify-start items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-2 p-4"
            >
              <div
                class="flex justify-between items-center self-stretch flex-grow-0 flex-shrink-0 relative"
              >
                <p
                  class="flex-grow-0 flex-shrink-0 text-sm font-semibold text-left text-white"
                >
                  Subscription Title
                </p>
                <svg
                  width="18"
                  height="19"
                  viewBox="0 0 18 19"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                  class="flex-grow-0 flex-shrink-0"
                  preserveAspectRatio="xMidYMid meet"
                >
                  <circle cx="9" cy="9.5" r="8.5" stroke="white" />
                </svg>
              </div>
              <p
                class="flex-grow-0 flex-shrink-0 w-[215px] text-xs text-left text-[#e5f3ff]"
              >
                Lorem ipsum dolor sit amet consectetur. A in aliquet a ac
                volutpat.
              </p>
            </div>
            <svg
              width="248"
              height="2"
              viewBox="0 0 248 2"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="flex-grow-0 flex-shrink-0"
              preserveAspectRatio="none"
            >
              <path d="M0.832031 1H247.832" stroke="#D9D9D9" />
            </svg>
            <div
              class="flex justify-start items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-2.5 p-4 bg-[#f9f9f9]"
            >
              <p
                class="flex-grow w-[113.67px] text-xs text-left text-[#9a9a9a]"
              >
                Learn more
              </p>
              <p
                class="flex-grow w-[113.67px] text-xs text-right text-[#232323]"
              >
                <span
                  class="flex-grow w-[113.67px] text-xs font-semibold text-right text-[#232323]"
                  >$10.99</span
                ><span
                  class="flex-grow w-[113.67px] text-xs text-right text-[#232323]"
                  >/month</span
                >
              </p>
            </div>
          </div>
        </div>
      </div>
      <div
        class="flex flex-col justify-start items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-4"
      >
        <p
          class="flex-grow-0 flex-shrink-0 text-lg font-semibold text-left text-[#232323]"
        >
          Payment
        </p>
        <div
          class="flex justify-start items-center self-stretch flex-grow-0 flex-shrink-0 relative gap-4"
        >
          <svg
            width="64"
            height="32"
            viewBox="0 0 64 32"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            class="flex-grow-0 flex-shrink-0 w-16 h-8 relative"
            preserveAspectRatio="xMidYMid meet"
          >
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M27.3943 27.1865L27.8305 24.5447L26.8588 24.5231H22.2188L25.4434 5.02771C25.4535 4.96867 25.4859 4.91387 25.5334 4.87489C25.581 4.8359 25.6418 4.81451 25.7053 4.81451H33.5291C36.1267 4.81451 37.9192 5.32978 38.8549 6.34695C39.2937 6.82413 39.5731 7.32291 39.7084 7.8716C39.8502 8.44746 39.8525 9.13538 39.7142 9.97456L39.7042 10.0356V10.5734L40.1429 10.8104C40.5123 10.9973 40.806 11.2112 41.0312 11.456C41.4064 11.8641 41.6492 12.3827 41.7518 12.9973C41.8578 13.6296 41.8228 14.3821 41.6492 15.234C41.449 16.2137 41.1254 17.0671 40.6882 17.7653C40.2864 18.4087 39.7743 18.9424 39.1661 19.3559C38.5855 19.7488 37.8958 20.0471 37.1159 20.2381C36.3601 20.4256 35.4985 20.5203 34.5534 20.5203H33.9445C33.5093 20.5203 33.0864 20.6698 32.7544 20.9378C32.4215 21.2113 32.2014 21.5851 32.1339 21.9939L32.0878 22.2319L31.3171 26.8884L31.2822 27.0593C31.2729 27.1134 31.257 27.1404 31.2336 27.1587C31.2129 27.1754 31.1829 27.1865 31.1537 27.1865H27.3943"
              fill="#28356A"
            />
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M40.5587 10.0978C40.5356 10.2401 40.5087 10.3856 40.4788 10.5351C39.4471 15.5862 35.917 17.3311 31.4088 17.3311H29.1133C28.5619 17.3311 28.0972 17.7127 28.0114 18.2314L26.5033 27.3527C26.4475 27.6933 26.7227 28.0001 27.083 28.0001H31.1543C31.6363 28.0001 32.0459 27.6661 32.1218 27.2128L32.1618 27.0157L32.9283 22.3773L32.9776 22.1229C33.0526 21.668 33.4631 21.3339 33.9451 21.3339H34.554C38.4985 21.3339 41.5865 19.807 42.489 15.3881C42.8659 13.5422 42.6708 12.0009 41.6732 10.9169C41.3713 10.5901 40.9968 10.3188 40.5587 10.0978"
              fill="#019DDE"
            />
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M39.4798 9.68737C39.3221 9.64348 39.1595 9.60383 38.9927 9.56796C38.8249 9.53299 38.6532 9.50202 38.4763 9.47484C37.8574 9.3795 37.1792 9.33427 36.4528 9.33427H30.3205C30.1694 9.33427 30.0259 9.3668 29.8976 9.42561C29.6147 9.55526 29.4047 9.81056 29.3537 10.1231L28.0491 18.0016L28.0117 18.2313C28.0975 17.7127 28.5622 17.3311 29.1136 17.3311H31.409C35.9173 17.3311 39.4473 15.5852 40.4791 10.535C40.5099 10.3855 40.5358 10.2401 40.559 10.0977C40.298 9.96561 40.0153 9.85266 39.7109 9.75643C39.6356 9.73259 39.5581 9.70964 39.4798 9.68737"
              fill="#00164C"
            />
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M29.353 10.1232C29.404 9.81061 29.614 9.55531 29.897 9.42655C30.0262 9.36752 30.1687 9.33499 30.3198 9.33499H36.4521C37.1785 9.33499 37.8567 9.38044 38.4756 9.47578C38.6525 9.50274 38.8242 9.53393 38.992 9.5689C39.1588 9.60455 39.3214 9.64442 39.4791 9.68809C39.5574 9.71036 39.635 9.73353 39.7109 9.75648C40.0153 9.85271 40.2983 9.96655 40.5592 10.0978C40.8662 8.23116 40.5567 6.96026 39.4983 5.80942C38.3313 4.5423 36.2253 4.00008 33.5302 4.00008H25.7062C25.1558 4.00008 24.6861 4.38168 24.6011 4.90118L21.3423 24.597C21.2781 24.9867 21.5933 25.3382 22.0054 25.3382H26.8356L29.353 10.1232"
              fill="#012F86"
            />
          </svg>
          <div
            class="flex flex-col justify-start items-start flex-grow relative gap-1"
          >
            <p
              class="flex-grow-0 flex-shrink-0 text-lg font-semibold text-left text-[#232323]"
            >
              Paypal
            </p>
            <p
              class="flex-grow-0 flex-shrink-0 text-sm text-left text-[#9a9a9a]"
            >
              ganteng@mail.com
            </p>
          </div>
          <button
            class="bg-transparent border-none"
            on:click={() => {
              show_modal = true;
            }}
          >
            <svg
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="flex-grow-0 flex-shrink-0 w-6 h-6 relative"
              preserveAspectRatio="none"
            >
              <path
                d="M13.2594 3.6L5.04936 12.29C4.73936 12.62 4.43936 13.27 4.37936 13.72L4.00936 16.96C3.87936 18.13 4.71936 18.93 5.87936 18.73L9.09936 18.18C9.54936 18.1 10.1794 17.77 10.4894 17.43L18.6994 8.74C20.1194 7.24 20.7594 5.53 18.5494 3.44C16.3494 1.37 14.6794 2.1 13.2594 3.6Z"
                stroke="#9A9A9A"
                stroke-width="1.5"
                stroke-miterlimit="10"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M11.8906 5.05C12.3206 7.81 14.5606 9.92 17.3406 10.2"
                stroke="#9A9A9A"
                stroke-width="1.5"
                stroke-miterlimit="10"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M3 22H21"
                stroke="#9A9A9A"
                stroke-width="1.5"
                stroke-miterlimit="10"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </button>
        </div>
      </div>
      <p
        class="flex-grow-0 flex-shrink-0 text-xs font-semibold text-left text-[#eb5842]"
      >
        Delete Account
      </p>
      <div
        class="flex justify-end items-start self-stretch flex-grow-0 flex-shrink-0 gap-3"
      >
        <div
          class="flex justify-center items-center flex-grow-0 flex-shrink-0 w-36 relative gap-2 p-4 bg-[#1f206c]"
        >
          <p
            class="flex-grow-0 flex-shrink-0 text-base font-medium text-center text-white"
          >
            Save Changes
          </p>
        </div>
      </div>
    </div>
    <div
      class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 w-[888px] gap-8 p-8 bg-white"
    >
      <div
        class="flex flex-col justify-start items-start self-stretch flex-grow-0 flex-shrink-0 gap-6"
      >
        <div
          class="flex flex-col justify-start items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-8"
        >
          <p
            class="flex-grow-0 flex-shrink-0 text-lg font-semibold text-left text-[#232323]"
          >
            Manage Team Members
          </p>
          <div
            class="flex justify-start items-end self-stretch flex-grow-0 flex-shrink-0 gap-4"
          >
            <div
              class="flex flex-col justify-start items-start flex-grow relative gap-2"
            >
              <p
                class="flex-grow-0 flex-shrink-0 w-[327px] text-sm font-semibold text-left text-[#232323]"
              >
                Email
              </p>
              <div
                class="flex flex-col justify-center items-center self-stretch flex-grow-0 flex-shrink-0 relative p-4 bg-[#e9e9f0] border border-[#1f206c]"
              >
                <p
                  class="self-stretch flex-grow-0 flex-shrink-0 w-[632px] text-lg font-medium text-left text-[#1f206c]"
                >
                  ganteng@mail.com
                </p>
              </div>
            </div>
            <div
              class="flex justify-center items-center flex-grow-0 flex-shrink-0 w-36 relative gap-2 p-4 bg-[#1f206c]"
            >
              <p
                class="flex-grow-0 flex-shrink-0 text-base font-medium text-center text-white"
              >
                Invite
              </p>
            </div>
          </div>
        </div>
        <div
          class="flex flex-col justify-start items-start self-stretch flex-grow-0 flex-shrink-0 gap-4"
        >
          <div
            class="flex justify-start items-center self-stretch flex-grow-0 flex-shrink-0 gap-8"
          >
            <div
              class="flex justify-start items-center flex-grow relative gap-4"
            >
              <img class="flex-grow-0 flex-shrink-0" src="ellipse-428.png" />
              <div
                class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 relative"
              >
                <p
                  class="flex-grow-0 flex-shrink-0 text-xs font-medium text-left text-[#232323]"
                >
                  Ganteng
                </p>
                <p
                  class="flex-grow-0 flex-shrink-0 text-xs text-left text-[#9a9a9a]"
                >
                  ganteng@mail.com
                </p>
              </div>
            </div>
            <div
              class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-2"
            >
              <p
                class="flex-grow-0 flex-shrink-0 text-xs font-medium text-left text-[#9a9a9a]"
              >
                Can view
              </p>
              <svg
                width="12"
                height="12"
                viewBox="0 0 12 12"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="flex-grow-0 flex-shrink-0 w-3 h-3 relative"
                preserveAspectRatio="xMidYMid meet"
              >
                <path
                  d="M9.95906 4.47498L6.69906 7.73498C6.31406 8.11998 5.68406 8.11998 5.29906 7.73498L2.03906 4.47498"
                  stroke="#9A9A9A"
                  stroke-width="1.5"
                  stroke-miterlimit="10"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
            </div>
            <div
              class="flex justify-start items-start flex-grow-0 flex-shrink-0 relative gap-2"
            >
              <svg
                width="18"
                height="18"
                viewBox="0 0 18 18"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="flex-grow-0 flex-shrink-0 w-[18px] h-[18px] relative"
                preserveAspectRatio="xMidYMid meet"
              >
                <path
                  d="M15.75 4.48499C13.2525 4.23749 10.74 4.10999 8.235 4.10999C6.75 4.10999 5.265 4.18499 3.78 4.33499L2.25 4.48499"
                  stroke="#EB5842"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M6.375 3.7275L6.54 2.745C6.66 2.0325 6.75 1.5 8.0175 1.5H9.9825C11.25 1.5 11.3475 2.0625 11.46 2.7525L11.625 3.7275"
                  stroke="#EB5842"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M14.1383 6.85498L13.6508 14.4075C13.5683 15.585 13.5008 16.5 11.4083 16.5H6.59328C4.50078 16.5 4.43328 15.585 4.35078 14.4075L3.86328 6.85498"
                  stroke="#EB5842"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M7.74805 12.375H10.2455"
                  stroke="#EB5842"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M7.125 9.375H10.875"
                  stroke="#EB5842"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
              <p
                class="flex-grow-0 flex-shrink-0 text-xs font-medium text-left text-[#eb5842]"
              >
                Delete
              </p>
            </div>
          </div>
          <div
            class="flex justify-start items-center self-stretch flex-grow-0 flex-shrink-0 gap-8"
          >
            <div
              class="flex justify-start items-center flex-grow relative gap-4"
            >
              <img class="flex-grow-0 flex-shrink-0" src="ellipse-428.png" />
              <div
                class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 relative"
              >
                <p
                  class="flex-grow-0 flex-shrink-0 text-xs font-medium text-left text-[#232323]"
                >
                  Ganteng
                </p>
                <p
                  class="flex-grow-0 flex-shrink-0 text-xs text-left text-[#9a9a9a]"
                >
                  ganteng@mail.com
                </p>
              </div>
            </div>
            <div
              class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-2"
            >
              <p
                class="flex-grow-0 flex-shrink-0 text-xs font-medium text-left text-[#9a9a9a]"
              >
                Can edit
              </p>
              <svg
                width="12"
                height="12"
                viewBox="0 0 12 12"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="flex-grow-0 flex-shrink-0 w-3 h-3 relative"
                preserveAspectRatio="xMidYMid meet"
              >
                <path
                  d="M9.95906 4.47498L6.69906 7.73498C6.31406 8.11998 5.68406 8.11998 5.29906 7.73498L2.03906 4.47498"
                  stroke="#9A9A9A"
                  stroke-width="1.5"
                  stroke-miterlimit="10"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
            </div>
            <div
              class="flex justify-start items-start flex-grow-0 flex-shrink-0 relative gap-2"
            >
              <svg
                width="18"
                height="18"
                viewBox="0 0 18 18"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="flex-grow-0 flex-shrink-0 w-[18px] h-[18px] relative"
                preserveAspectRatio="xMidYMid meet"
              >
                <path
                  d="M15.75 4.48499C13.2525 4.23749 10.74 4.10999 8.235 4.10999C6.75 4.10999 5.265 4.18499 3.78 4.33499L2.25 4.48499"
                  stroke="#EB5842"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M6.375 3.7275L6.54 2.745C6.66 2.0325 6.75 1.5 8.0175 1.5H9.9825C11.25 1.5 11.3475 2.0625 11.46 2.7525L11.625 3.7275"
                  stroke="#EB5842"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M14.1383 6.85498L13.6508 14.4075C13.5683 15.585 13.5008 16.5 11.4083 16.5H6.59328C4.50078 16.5 4.43328 15.585 4.35078 14.4075L3.86328 6.85498"
                  stroke="#EB5842"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M7.74805 12.375H10.2455"
                  stroke="#EB5842"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M7.125 9.375H10.875"
                  stroke="#EB5842"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
              <p
                class="flex-grow-0 flex-shrink-0 text-xs font-medium text-left text-[#eb5842]"
              >
                Delete
              </p>
            </div>
          </div>
          <div
            class="flex justify-start items-center self-stretch flex-grow-0 flex-shrink-0 gap-8"
          >
            <div
              class="flex justify-start items-center flex-grow relative gap-4"
            >
              <img class="flex-grow-0 flex-shrink-0" src="ellipse-428.png" />
              <div
                class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 relative"
              >
                <p
                  class="flex-grow-0 flex-shrink-0 text-xs font-medium text-left text-[#232323]"
                >
                  Ganteng
                </p>
                <p
                  class="flex-grow-0 flex-shrink-0 text-xs text-left text-[#9a9a9a]"
                >
                  ganteng@mail.com
                </p>
              </div>
            </div>
            <div
              class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-2"
            >
              <p
                class="flex-grow-0 flex-shrink-0 text-xs font-medium text-left text-[#9a9a9a]"
              >
                Can edit
              </p>
              <svg
                width="12"
                height="12"
                viewBox="0 0 12 12"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="flex-grow-0 flex-shrink-0 w-3 h-3 relative"
                preserveAspectRatio="xMidYMid meet"
              >
                <path
                  d="M9.95906 4.47498L6.69906 7.73498C6.31406 8.11998 5.68406 8.11998 5.29906 7.73498L2.03906 4.47498"
                  stroke="#9A9A9A"
                  stroke-width="1.5"
                  stroke-miterlimit="10"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
            </div>
            <div
              class="flex justify-start items-start flex-grow-0 flex-shrink-0 relative gap-2"
            >
              <svg
                width="18"
                height="18"
                viewBox="0 0 18 18"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="flex-grow-0 flex-shrink-0 w-[18px] h-[18px] relative"
                preserveAspectRatio="xMidYMid meet"
              >
                <path
                  d="M15.75 4.48499C13.2525 4.23749 10.74 4.10999 8.235 4.10999C6.75 4.10999 5.265 4.18499 3.78 4.33499L2.25 4.48499"
                  stroke="#EB5842"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M6.375 3.7275L6.54 2.745C6.66 2.0325 6.75 1.5 8.0175 1.5H9.9825C11.25 1.5 11.3475 2.0625 11.46 2.7525L11.625 3.7275"
                  stroke="#EB5842"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M14.1383 6.85498L13.6508 14.4075C13.5683 15.585 13.5008 16.5 11.4083 16.5H6.59328C4.50078 16.5 4.43328 15.585 4.35078 14.4075L3.86328 6.85498"
                  stroke="#EB5842"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M7.74805 12.375H10.2455"
                  stroke="#EB5842"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M7.125 9.375H10.875"
                  stroke="#EB5842"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
              <p
                class="flex-grow-0 flex-shrink-0 text-xs font-medium text-left text-[#eb5842]"
              >
                Delete
              </p>
            </div>
          </div>
        </div>
        <div
          class="flex justify-center items-center self-stretch flex-grow-0 flex-shrink-0 relative gap-2 p-3 bg-[#e9e9e9]"
        >
          <p
            class="flex-grow-0 flex-shrink-0 text-sm font-medium text-center text-[#232323]"
          >
            Show All Team Members
          </p>
        </div>
      </div>
    </div>
  </div>
</div>
{#if show_modal}
  <Modal
    on:close={(event) => {
      show_modal = false;
    }}
  >
    <div
      class="flex flex-col justify-start items-center flex-grow-0 flex-shrink-0 relative gap-6 px-8 pt-8 pb-[72px] bg-white"
    >
      <div
        class="flex justify-between items-center self-stretch flex-grow-0 flex-shrink-0 relative"
      >
        <div
          class="flex justify-start items-center self-stretch flex-grow-0 flex-shrink-0 w-[182px] relative gap-4"
        >
          <svg
            width="25"
            height="24"
            viewBox="0 0 25 24"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            class="flex-grow-0 flex-shrink-0 w-6 h-6 relative"
            preserveAspectRatio="none"
          >
            <path
              d="M10.07 5.92999L4 12L10.07 18.07"
              stroke="#232323"
              stroke-width="1.5"
              stroke-miterlimit="10"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
            <path
              d="M20.9999 12H4.16992"
              stroke="#232323"
              stroke-width="1.5"
              stroke-miterlimit="10"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </svg>
          <p
            class="flex-grow-0 flex-shrink-0 text-lg font-semibold text-left text-[#232323]"
          >
            Change Payment
          </p>
        </div>
        <svg
          width="25"
          height="24"
          viewBox="0 0 25 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          class="flex-grow-0 flex-shrink-0 w-6 h-6 relative"
          preserveAspectRatio="none"
        >
          <path
            d="M5.5 5L19.4991 18.9991"
            stroke="#232323"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M5.50094 18.9991L19.5 5"
            stroke="#232323"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>
      </div>
      <div
        class="flex justify-start items-center flex-grow-0 flex-shrink-0 w-[757px] gap-4"
      >
        <div
          class="flex justify-start items-center flex-grow gap-4 p-4 bg-white border border-[#1f206c]"
        >
          <div class="flex justify-start items-center flex-grow relative gap-4">
            <svg
              width="49"
              height="25"
              viewBox="0 0 49 25"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="flex-grow-0 flex-shrink-0 w-12 h-6 relative"
              preserveAspectRatio="none"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M21.0457 20.8899L21.3729 18.9085L20.6441 18.8923H17.1641L19.5826 4.27078C19.5901 4.2265 19.6145 4.1854 19.65 4.15616C19.6858 4.12693 19.7313 4.11089 19.779 4.11089H25.6468C27.595 4.11089 28.9394 4.49734 29.6412 5.26022C29.9702 5.6181 30.1798 5.99219 30.2813 6.4037C30.3876 6.8356 30.3894 7.35153 30.2857 7.98092L30.2781 8.0267V8.43002L30.6072 8.60779C30.8842 8.74797 31.1045 8.90837 31.2734 9.09199C31.5548 9.39807 31.7369 9.78703 31.8138 10.248C31.8934 10.7222 31.8671 11.2866 31.7369 11.9255C31.5867 12.6603 31.344 13.3004 31.0162 13.824C30.7148 14.3065 30.3307 14.7068 29.8746 15.0169C29.4391 15.3116 28.9219 15.5354 28.3369 15.6785C27.7701 15.8192 27.1238 15.8902 26.415 15.8902H25.9584C25.632 15.8902 25.3148 16.0023 25.0658 16.2033C24.8161 16.4085 24.651 16.6889 24.6004 16.9955L24.5659 17.1739L23.9878 20.6663L23.9617 20.7945C23.9547 20.8351 23.9428 20.8553 23.9252 20.869C23.9096 20.8815 23.8872 20.8899 23.8653 20.8899H21.0457"
                fill="#28356A"
              />
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M30.918 8.07333C30.9007 8.18009 30.8805 8.28919 30.8581 8.4013C30.0843 12.1896 27.4368 13.4984 24.0556 13.4984H22.334C21.9204 13.4984 21.5719 13.7846 21.5076 14.1735L20.3765 21.0145C20.3346 21.27 20.541 21.5001 20.8112 21.5001H23.8648C24.2263 21.5001 24.5334 21.2496 24.5904 20.9096L24.6204 20.7617L25.1953 17.283L25.2323 17.0922C25.2885 16.751 25.5964 16.5004 25.9579 16.5004H26.4145C29.3729 16.5004 31.6889 15.3553 32.3658 12.0411C32.6484 10.6567 32.5021 9.50067 31.7539 8.68767C31.5275 8.44257 31.2466 8.23907 30.918 8.07333"
                fill="#019DDE"
              />
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M30.1089 7.76553C29.9906 7.73261 29.8686 7.70287 29.7435 7.67597C29.6177 7.64974 29.4889 7.62652 29.3563 7.60614C28.8921 7.53463 28.3834 7.50071 27.8386 7.50071H23.2394C23.126 7.50071 23.0185 7.5251 22.9223 7.56921C22.7101 7.66645 22.5525 7.85792 22.5143 8.09233L21.5358 14.0012L21.5078 14.1735C21.5721 13.7845 21.9206 13.4983 22.3342 13.4983H24.0558C27.437 13.4983 30.0845 12.1889 30.8583 8.40126C30.8815 8.28915 30.9009 8.18005 30.9183 8.07329C30.7225 7.97421 30.5105 7.8895 30.2822 7.81732C30.2258 7.79945 30.1676 7.78224 30.1089 7.76553"
                fill="#00164C"
              />
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M22.5143 8.09237C22.5525 7.85796 22.71 7.66649 22.9222 7.56992C23.0191 7.52564 23.126 7.50125 23.2394 7.50125H27.8386C28.3834 7.50125 28.8921 7.53533 29.3562 7.60684C29.4889 7.62706 29.6177 7.65045 29.7435 7.67668C29.8686 7.70341 29.9906 7.73332 30.1089 7.76607C30.1676 7.78278 30.2257 7.80015 30.2827 7.81736C30.511 7.88954 30.7232 7.97492 30.9189 8.07332C31.1492 6.67338 30.917 5.7202 30.1232 4.85707C29.248 3.90673 27.6685 3.50006 25.6472 3.50006H19.7792C19.3663 3.50006 19.0141 3.78627 18.9503 4.17589L16.5063 18.9478C16.4581 19.24 16.6944 19.5036 17.0036 19.5036H20.6262L22.5143 8.09237"
                fill="#012F86"
              />
            </svg>
            <p
              class="flex-grow-0 flex-shrink-0 text-base font-semibold text-left text-[#232323]"
            >
              Paypal
            </p>
          </div>
          <div
            class="flex justify-start items-start flex-grow-0 flex-shrink-0 relative gap-2.5 p-1 rounded-[100px] border-2 border-[#1f206c]"
          >
            <svg
              width="12"
              height="13"
              viewBox="0 0 12 13"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="flex-grow-0 flex-shrink-0"
              preserveAspectRatio="xMidYMid meet"
            >
              <circle cx="6" cy="6.5" r="6" fill="#1F206C" />
            </svg>
          </div>
        </div>
        <div class="flex justify-start items-center flex-grow gap-4 p-4">
          <div class="flex justify-start items-center flex-grow relative gap-4">
            <svg
              width="48"
              height="25"
              viewBox="0 0 48 25"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="flex-grow-0 flex-shrink-0 w-12 h-6 relative"
              preserveAspectRatio="none"
            >
              <rect y="0.5" width="48" height="24" rx="2" fill="#635BFF" />
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M25.1729 8.09906L23.1957 8.52443V6.91749L25.1729 6.5V8.09906ZM17.1382 7.41375L15.2162 7.82336L15.2083 14.133C15.2083 15.2988 16.0827 16.1574 17.2485 16.1574C17.8944 16.1574 18.367 16.0392 18.627 15.8975V14.2984C18.3749 14.4008 17.1303 14.7631 17.1303 13.5973V10.8009H18.627V9.1231H17.1303L17.1382 7.41375ZM12.4828 10.6985C12.0653 10.6985 11.8132 10.8167 11.8132 11.1239C11.8132 11.4593 12.2471 11.6069 12.7852 11.7899C13.6626 12.0883 14.8174 12.4811 14.8223 13.936C14.8223 15.3461 13.6959 16.1574 12.0574 16.1574C11.38 16.1574 10.6395 16.0235 9.90696 15.7084V13.8336C10.5686 14.196 11.4036 14.4638 12.0574 14.4638C12.4986 14.4638 12.8136 14.3457 12.8136 13.9833C12.8136 13.6118 12.3434 13.4419 11.7756 13.2369C10.911 12.9247 9.82031 12.5308 9.82031 11.2184C9.82031 9.82416 10.8837 8.98918 12.4828 8.98918C13.1366 8.98918 13.7825 9.09159 14.4363 9.35153V11.2027C13.8377 10.8797 13.0815 10.6985 12.4828 10.6985ZM35.3344 8.98918C37.2013 8.98918 38.1781 10.5804 38.1781 12.5969C38.1781 12.7058 38.1729 12.8878 38.1684 13.0422L38.1684 13.0423V13.0423L38.1684 13.0427C38.1652 13.1562 38.1623 13.2546 38.1623 13.298H34.3104C34.3971 14.2275 35.0745 14.4953 35.8386 14.4953C36.6184 14.4953 37.2328 14.3299 37.7685 14.0621V15.6375C37.2328 15.9368 36.5239 16.1495 35.5865 16.1495C33.6645 16.1495 32.3254 14.9522 32.3254 12.5812C32.3254 10.5804 33.4597 8.98918 35.3344 8.98918ZM35.3266 10.5882C34.8303 10.5882 34.2868 10.9585 34.2868 11.8486H36.3191C36.3191 10.9585 35.8071 10.5882 35.3266 10.5882ZM21.0768 9.70601L20.9507 9.1231H19.2493V16.0156H21.2186V11.3445C21.6833 10.7379 22.471 10.8482 22.7152 10.9348V9.1231C22.4632 9.02857 21.5415 8.85527 21.0768 9.70601ZM25.1729 9.12309H23.1957V16.0156H25.1729V9.12309ZM29.2848 8.98918C28.5128 8.98918 28.0166 9.35153 27.7409 9.6036L27.6385 9.11522H25.9055V18.3L27.8748 17.8825L27.8826 15.6533C28.1662 15.8581 28.5837 16.1495 29.2769 16.1495C30.6869 16.1495 31.9709 15.0152 31.9709 12.5182C31.963 10.2338 30.6633 8.98918 29.2848 8.98918ZM28.8121 14.4165C28.3474 14.4165 28.0717 14.2511 27.8826 14.0463L27.8748 11.1239C28.0796 10.8955 28.3631 10.7379 28.8121 10.7379C29.529 10.7379 30.0252 11.5414 30.0252 12.5733C30.0252 13.6288 29.5368 14.4165 28.8121 14.4165Z"
                fill="#FBFAF8"
              />
            </svg>
            <p
              class="flex-grow-0 flex-shrink-0 text-base font-semibold text-left text-[#232323]"
            >
              Stripe
            </p>
          </div>
          <div
            class="flex justify-start items-start flex-grow-0 flex-shrink-0 relative gap-2.5 rounded-[100px]"
          >
            <svg
              width="21"
              height="21"
              viewBox="0 0 21 21"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="flex-grow-0 flex-shrink-0"
              preserveAspectRatio="xMidYMid meet"
            >
              <circle
                cx="10.5"
                cy="10.5"
                r="8.5"
                stroke="#D9D9D9"
                stroke-width="3"
              />
            </svg>
          </div>
        </div>
      </div>
      <svg
        width="758"
        height="1"
        viewBox="0 0 758 1"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        class="self-stretch flex-grow-0 flex-shrink-0"
        preserveAspectRatio="none"
      >
        <path d="M0.5 0.5H757.5" stroke="#D9D9D9" />
      </svg>
      <div
        class="flex flex-col justify-start items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-2"
      >
        <p
          class="flex-grow-0 flex-shrink-0 w-[327px] text-sm font-semibold text-left text-[#232323]"
        >
          Email
        </p>
        <div
          class="flex flex-col justify-center items-center self-stretch flex-grow-0 flex-shrink-0 relative p-4 bg-white border border-[#1f206c]"
        >
          <p
            class="self-stretch flex-grow-0 flex-shrink-0 w-[725px] text-lg font-medium text-left text-[#1f206c]"
          >
            ganteng@mail.com
          </p>
        </div>
      </div>
      <div
        class="flex justify-end items-start self-stretch flex-grow-0 flex-shrink-0 gap-3"
      >
        <div
          class="flex justify-center items-center flex-grow-0 flex-shrink-0 w-36 relative gap-2 p-4 border border-[#1f206c]"
        >
          <p
            class="flex-grow-0 flex-shrink-0 text-base font-medium text-center text-[#232323]"
          >
            Discard
          </p>
        </div>
        <div
          class="flex justify-center items-center flex-grow-0 flex-shrink-0 w-36 relative gap-2 p-4 bg-[#1f206c]"
        >
          <p
            class="flex-grow-0 flex-shrink-0 text-base font-medium text-center text-white"
          >
            Save
          </p>
        </div>
      </div>
    </div>
  </Modal>
{/if}
