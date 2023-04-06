<script>
  // @ts-nocheck

  import { onMount } from "svelte";
  import image_40 from "../../../assets/40.png";
  import image_41 from "../../../assets/41.png";
  import image_42 from "../../../assets/42.png";
  import image_43 from "../../../assets/43.png";
  import image_44 from "../../../assets/44.png";
  import Overlay from "../overlay.svelte";

  const data = [
    {
      name: "Richard Morris",
      role: "Sr. Full Stack Developer",
      image: image_40,
    },
    {
      name: "Nat Wollny",
      role: "Co-Founder and CEO",
      image: image_41,
    },
    {
      name: "Rodrigo Mello",
      role: "Machine Learning Scientist",
      image: image_42,
    },
    {
      name: "Christoph Sträter",
      role: "Co-Founder and CTO",
      image: image_43,
    },
    {
      name: "Interested in joining?",
      role: "Open application",
      image: image_44,
    },
  ];
  let slide_width = 60;

  function slideItem(container, direction) {
    // Get the current position of the container
    const currentPosition = container.scrollLeft;

    // Get the width of the container
    const containerWidth = container.offsetWidth;
    // get the scrolled percentage of container

    // Calculate the new position based on the direction
    const newPosition =
      direction === "left"
        ? currentPosition - containerWidth / 3
        : currentPosition + containerWidth / 3;

    // Animate the slide
    container.scrollTo({
      left: newPosition,
      behavior: "smooth",
    });

    if (direction === "left") {
      if (slide_width > 60) slide_width = slide_width - 11;
    } else {
      if (slide_width < 100) slide_width = slide_width + 11;
    }

    // Calculate the percentage of the container that has been scrolled
    // set width of slide indicator max should be 252px
    const { scrollWidth, scrollLeft, clientWidth } = container;

    // Calculate the percentage of the scroll position
    const scrollPercentage = (scrollLeft / (scrollWidth - clientWidth)) * 100;

    const slide_indicator = document.querySelector(".slide-indicator");
    slide_indicator.style.width = `${scrollPercentage}%`;
  }

  onMount(() => {
    const container = document.querySelector(".slide-container");
    const leftButton = document.querySelector(".arrow-left");
    const rightButton = document.querySelector(".arrow-right");

    container.onscroll = function () {
      const { scrollWidth, scrollLeft, clientWidth } = container;
      const scrollPercentage = (scrollLeft / (scrollWidth - clientWidth)) * 100;
      const slide_indicator = document.querySelector(".slide-indicator");
      slide_indicator.style.width = `${scrollPercentage}%`;
    };

    function scrollLeft(offset) {
      // Calculate the new scrollLeft value
      const scrollable = container;
      const newScrollLeft = scrollable.scrollLeft + offset;

      // Scroll to the new position with smooth behavior
      scrollable.scrollTo({
        left: newScrollLeft,
        behavior: "smooth",
      });

      // Calculate the percentage of the scroll position
      const { scrollWidth, clientWidth } = scrollable;
      const scrollPercentage =
        (newScrollLeft / (scrollWidth - clientWidth)) * 100;

      // Set the width of the indicator to the scroll percentage
      const slide_indicator = document.querySelector(".slide-indicator");

      slide_indicator.style.width = `${scrollPercentage}%`;
    }

    leftButton.addEventListener("click", () => {
      // slideItem(container, "left");
      scrollLeft(-440);
    });

    rightButton.addEventListener("click", () => {
      scrollLeft(440);
    });
  });
</script>

<div
  id="team"
  class="flex flex-col justify-start items-end self-stretch overflow-hidden gap-[66px] pl-[68px] py-[39px] bg-white border-t-0 border-r-0 border-b border-l-0 border-[#232323]/[0.16]"
>
  <div class="flex justify-start items-start self-stretch relative gap-[473px]">
    <div class="flex flex-col justify-start items-start relative gap-6">
      <span
        class="flex-grow-0 flex-shrink-0 text-lg font-semibold text-left text-[#1f206c]"
      >
        TEAM
      </span>
      <p
        class="flex-grow-0 flex-shrink-0 text-[58px] text-left uppercase text-neutral-900"
      >
        the team
      </p>
    </div>
    <span
      class="flex-grow-0 flex-shrink-0 w-[610px] text-lg text-left text-[#757575]"
    >
      We are gamers, physicists, biologists, fashionistas and generative
      enthusiasts. United to bring cutting edge creative technologies to content
      creators.
    </span>
  </div>

  <div
    class="flex justify-start items-start self-stretch relative overflow-y-hidden hide-scrollbar py-4 px-2 gap-[42px] slide-container"
  >
    {#each data as { name, role, image }}
      <div class="group relative min-w-[396px] overflow-hidden">
        <img
          src={image}
          alt="..."
          class="object-cover h-[600px] group-hover:blur-3xl"
        />
        <Overlay>
          <div
            class="flex flex-col justify-between items-center h-full w-full p-10"
          >
            <div class="flex flex-col justify-start items-start relative">
              <span
                class="flex-grow-0 flex-shrink-0 text-[32px] font-semibold text-left text-white"
              >
                {name}
              </span>
              <span
                class="flex-grow-0 flex-shrink-0 w-[312px] text-lg text-left text-white"
              >
                {role}
              </span>
            </div>
            <div class="flex flex-col justify-start items-start gap-2">
              {#each ["Medium", "Twitter", "LinkedIn"] as media}
                <div
                  class="flex justify-center items-center w-[312px] relative gap-3 px-8 py-4 bg-white"
                >
                  <span
                    class="flex-grow-0 flex-shrink-0 text-lg font-medium text-left text-[#1f206c]"
                  >
                    {media}
                  </span>
                  <svg
                    width="22"
                    height="15"
                    viewBox="0 0 22 15"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                    class="flex-grow-0 flex-shrink-0"
                    preserveAspectRatio="none"
                  >
                    <path
                      d="M1.55078 7.5H18.3808M14.3808 1.42999L20.4508 7.49999L14.3808 13.57"
                      stroke="#1F206C"
                      stroke-width="1.5"
                      stroke-miterlimit="10"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </svg>
                </div>
              {/each}
            </div>
          </div>
        </Overlay>
      </div>
    {/each}
  </div>
  <div class="flex justify-start items-center relative gap-5 pr-[68px]">
    <div
      class="flex justify-start items-start relative w-[252px] overflow-x-hidden"
    >
      <div
        class="flex-grow-0 flex-shrink-0 slide-indicator h-[3px] bg-[#4434c9]"
      />
      <div class="flex-grow-0 flex-shrink-0 h-[3px] w-[252px] bg-[#f4f4f4]" />
    </div>
    <svg
      width="24"
      height="25"
      viewBox="0 0 24 25"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
      class="flex-grow-0 flex-shrink-0 w-6 h-6 relative arrow-left"
      preserveAspectRatio="none"
    >
      <path
        d="M9.57 6.07941L3.5 12.1494L9.57 18.2194"
        stroke="#757575"
        stroke-width="1.5"
        stroke-miterlimit="10"
        stroke-linecap="round"
        stroke-linejoin="round"
      />
      <path
        d="M20.4999 12.1494H3.66992"
        stroke="#757575"
        stroke-width="1.5"
        stroke-miterlimit="10"
        stroke-linecap="round"
        stroke-linejoin="round"
      />
    </svg>
    <svg
      width="24"
      height="25"
      viewBox="0 0 24 25"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
      class="flex-grow-0 flex-shrink-0 w-6 h-6 relative arrow-right"
      preserveAspectRatio="none"
    >
      <path
        d="M14.4297 6.07941L20.4997 12.1494L14.4297 18.2194"
        stroke="#4434C9"
        stroke-width="1.5"
        stroke-miterlimit="10"
        stroke-linecap="round"
        stroke-linejoin="round"
      />
      <path
        d="M3.5 12.1494H20.33"
        stroke="#4434C9"
        stroke-width="1.5"
        stroke-miterlimit="10"
        stroke-linecap="round"
        stroke-linejoin="round"
      />
    </svg>
  </div>
</div>

<style>
  .slide-container::-webkit-scrollbar {
    display: none;
  }
</style>
