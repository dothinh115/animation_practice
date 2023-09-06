<template>
  <main class="overflow-x-hidden bg-slate-900">
    <section>
      <div class="pt-[50px] min-h-[1000px] px-16 text-white">
        <h1 class="text-[45px] font-bold tracking-wide">GSAP PRACTICE</h1>
      </div>
    </section>
    <section>
      <div class="px-16 text-white my-16">
        <h2 class="text-[45px] font-bold tracking-wide">SECTION 1</h2>
      </div>
      <div class="relative">
        <div class="flex justify-center items-center gap-8 firstSection">
          <div class="min-w-[123px] h-[185px] rounded-[6px] overflow-hidden">
            <img src="/images/1_1.jpg" class="w-full h-full object-cover" />
          </div>
          <div class="min-w-[155px] h-[232px] rounded-[6px] overflow-hidden">
            <img src="/images/1_2.jpg" class="w-full h-full object-cover" />
          </div>
          <div class="min-w-[310px] h-[465px] rounded-[6px] overflow-hidden">
            <img src="/images/1_3.jpg" class="w-full h-full object-cover" />
          </div>
          <div
            class="w-[465px] h-[650px] min-h-[650px] aspect-w-3 aspect-h-5 rounded-[6px] overflow-hidden flex-shrink-0 firstSectionMainImg"
          >
            <img src="/images/1_main.jpg" class="w-full h-full object-cover" />
          </div>
          <div class="min-w-[310px] h-[465px] rounded-[6px] overflow-hidden">
            <img src="/images/1_4.jpg" class="w-full h-full object-cover" />
          </div>
          <div class="min-w-[155px] h-[232px] rounded-[6px] overflow-hidden">
            <img src="/images/1_5.jpg" class="w-full h-full object-cover" />
          </div>
          <div class="min-w-[123px] h-[185px] rounded-[6px] overflow-hidden">
            <img src="/images/1_6.jpg" class="w-full h-full object-cover" />
          </div>
        </div>
        <div class="px-16 text-white firstSectionText">
          <p class="text-[20px] font-semibold tracking-wide w-[450px]">
            Within this meticulously arranged AI-generated ensemble lies a
            tantalizing facade, captivating our gaze. Yet, as we search for the
            soul of human expression, we question whether algorithms can truly
            embody the essence of authentic art.
          </p>
        </div>
      </div>
    </section>
    <section class="mt-[500px]">
      <div class="px-16 text-white my-16">
        <h2 class="text-[45px] font-bold tracking-wide">SECTION 2</h2>
      </div>
      <div class="relative overflow-hidden secondSection">
        <div class="absolute w-full h-full secondSectionMoveTo"></div>
        <div
          class="relative w-screen h-screen grid grid-cols-3 grid-rows-3 gap-x-[calc(2.5vw)] gap-y-[calc(3vh)] overflow-hidden secondSectionNeededToFit"
        >
          <div
            class="w-full h-full rounded-[6px] overflow-hidden min-h-fit min-w-fit"
          >
            <img src="/images/2_1.jpg" class="w-full h-full" />
          </div>
          <div
            class="w-full h-full rounded-[6px] overflow-hidden min-h-fit min-w-fit"
          >
            <img src="/images/2_2.jpg" class="w-full h-full" />
          </div>
          <div
            class="w-full h-full rounded-[6px] overflow-hidden min-h-fit min-w-fit"
          >
            <img src="/images/2_3.jpg" class="w-full h-full object-cover" />
          </div>
          <div
            class="w-full h-full rounded-[6px] overflow-hidden min-h-fit min-w-fit"
          >
            <img src="/images/2_4.jpg" class="w-full h-full" />
          </div>
          <div
            class="w-full h-full rounded-[6px] overflow-hidden z-50 secondSectionMainImg"
          >
            <img src="/images/2_main.jpg" class="w-full h-full object-cover" />
          </div>
          <div
            class="w-full h-full rounded-[6px] overflow-hidden min-h-fit min-w-fit"
          >
            <img src="/images/2_5.jpg" class="w-full h-full" />
          </div>
          <div
            class="w-full h-full rounded-[6px] overflow-hidden min-h-fit min-w-fit"
          >
            <img src="/images/2_6.jpg" class="w-full h-full" />
          </div>
          <div
            class="w-full h-full rounded-[6px] overflow-hidden min-h-fit min-w-fit"
          >
            <img src="/images/2_7.jpg" class="w-full h-full" />
          </div>
          <div
            class="w-full h-full rounded-[6px] overflow-hidden min-h-fit min-w-fit"
          >
            <img src="/images/2_8.jpg" class="w-full h-full" />
          </div>
        </div>
      </div>
      <div class="px-16 text-white secondSectionText">
        <p class="text-[20px] font-semibold tracking-wide w-[450px]">
          Within this meticulously arranged AI-generated ensemble lies a
          tantalizing facade, captivating our gaze. Yet, as we search for the
          soul of human expression, we question whether algorithms can truly
          embody the essence of authentic art.
        </p>
      </div>
    </section>
    <section class="mt-[500px]">
      <div class="px-16 text-white my-16">
        <h2 class="text-[45px] font-bold tracking-wide">SECTION 3</h2>
      </div>
      <div
        class="relative grid grid-cols-10 grid-rows-4 w-screen h-[calc(70vh)] gap-8 thirdSection"
      >
        <div
          class="h-full w-full rounded-[6px] overflow-hidden item"
          v-for="(item, index) in thirdSectionDataObj.cols *
          thirdSectionDataObj.rows"
          :key="index"
        ></div>
        <div
          class="absolute top-1/2 -translate-y-1/2 left-1/2 -translate-x-1/2 w-[300px] h-[500px] thirdSectionMain"
        ></div>
      </div>
      <div class="px-16 text-white thirdSectionText h-[500px]">
        <p
          class="text-[60px] font-bold tracking-wide text-center h-full flex items-center justify-center"
        >
          The Art of Perfection?
        </p>
      </div>
    </section>
    <section class="mt-[500px]">
      <div class="px-16 text-white my-16">
        <h2 class="text-[45px] font-bold tracking-wide">SECTION 4</h2>
      </div>
      <div class="relative fourthSection">
        <div class="relative flex w-max gap-8 px-8">
          <div
            class="relative item w-[450px] h-[650px]"
            v-for="(item, index) in 6"
            :key="index"
          >
            <img
              :src="`/images/4_${index + 1}.jpg`"
              class="w-full h-full rounded-[32px]"
            />
          </div>
          <div class="fourthSectionText w-[450px] h-[650px]">
            <p
              class="text-[30px] font-semibold tracking-wide w-[600px] flex items-center h-full -translate-x-[200px] text-gray-500"
            >
              AI-generated art captivates with varied creations, sometimes
              senseless, yet impressively enigmatic.
            </p>
          </div>
        </div>
      </div>
    </section>

    <section class="mt-[500px]">
      <div class="px-16 text-white my-16">
        <h2 class="text-[45px] font-bold tracking-wide">SECTION 5</h2>
      </div>
      <div class="relative fifthSection">
        <div class="relative flex w-max gap-8 px-8">
          <div
            class="relative item w-[450px] h-[650px]"
            v-for="(item, index) in 6"
            :key="index"
          >
            <img
              :src="`/images/3_${index + 1}.jpg`"
              class="w-full h-full rounded-[32px]"
            />
          </div>
          <div class="fifthSectionText w-[450px] h-[650px]">
            <p
              class="text-[30px] font-semibold tracking-wide w-[600px] flex items-center h-full -translate-x-[200px] text-gray-500"
            >
              AI-generated art captivates with varied creations, sometimes
              senseless, yet impressively enigmatic.
            </p>
          </div>
        </div>
      </div>
    </section>

    <section class="mt-[500px]">
      <div class="px-16 text-white my-16">
        <h2 class="text-[45px] font-bold tracking-wide">SECTION 6</h2>
      </div>
      <div class="relative sixthSection">
        <div class="relative flex w-max gap-8 px-8">
          <div
            class="relative item w-[450px] h-[650px]"
            v-for="(item, index) in 6"
            :key="index"
          >
            <img
              :src="`/images/1_${index + 1}.jpg`"
              class="w-full h-full rounded-[32px]"
            />
          </div>
          <div class="sixthSectionText w-[450px] h-[650px]">
            <p
              class="text-[30px] font-semibold tracking-wide w-[600px] flex items-center h-full -translate-x-[200px] text-gray-500"
            >
              AI-generated art captivates with varied creations, sometimes
              senseless, yet impressively enigmatic.
            </p>
          </div>
        </div>
      </div>
    </section>

    <section class="mt-[500px]">
      <div class="px-16 text-white my-16">
        <h2 class="text-[45px] font-bold tracking-wide">SECTION 7</h2>
      </div>
      <div class="relative seventhSection w-screen h-screen overflow-hidden">
        <div
          class="sBackground grid gap-8"
          :class="`grid-cols-${seventhSectionDataObj.cols} grid-rows-${seventhSectionDataObj.rows}`"
        >
          <div
            class="w-full h-full"
            v-for="(item, index) in seventhSectionDataObj.cols *
              seventhSectionDataObj.rows +
            10"
            :key="index"
          >
            <img
              :src="`/images/7_${
                Number(index.toString().split('').slice(-1)) + 1
              }.jpeg`"
              class="w-full h-full"
            />
          </div>
        </div>
        <div
          class="absolute top-1/2 -translate-x-1/2 left-1/2 -translate-y-1/2 w-fit text-white text-[80px] font-light"
        >
          What is creativity?
        </div>
      </div>
    </section>

    <section class="mt-[500px]">
      <div class="px-16 text-white my-16">
        <h2 class="text-[45px] font-bold tracking-wide">SECTION 8</h2>
      </div>
    </section>
    <section class="h-[5000px]"></section>
  </main>
</template>
<script setup lang="ts">
import { gsap } from "gsap";
import { ScrollTrigger } from "gsap/ScrollTrigger";
import { Flip } from "gsap/Flip";

let secondSectionDataObj: {
    width: number;
    height: number;
  },
  thirdSectionDataObj: {
    items: number;
    cols: number;
    rows: number;
  } = {
    cols: 10,
    rows: 4,
    items: 16,
  },
  seventhSectionDataObj: { cols: number; rows: number } = {
    cols: 10,
    rows: 5,
  };

const thirdSectionImgsAdd = () => {
  const divArr = document.querySelectorAll(".thirdSection .item") || [];
  const randomPosition: Set<number> = new Set();
  while (Array.from(randomPosition).length < 16) {
    const randomPos = Math.floor(
      Math.random() * thirdSectionDataObj.cols * thirdSectionDataObj.rows
    ); // 0 - 39
    randomPosition.add(randomPos);
  }
  const randomPositionArr = Array.from(randomPosition);
  for (let position = 0; position < randomPositionArr.length; position++) {
    divArr[randomPositionArr[position]].innerHTML = `<img src="../images/3_${
      position + 1
    }.jpg" class="h-full w-full object-cover rounded-[6px] z-[${
      randomPositionArr[position]
    }]" />`;
  }
};

const updateSecondSectionPos = (progress: number) => {
  const secondSectionDivs =
    document.querySelectorAll(".secondSection div") || [];
  const translateX =
    (window.innerWidth - secondSectionDataObj.width) * progress * 1.1;
  const translateY =
    (window.innerHeight - secondSectionDataObj.height) * progress * 1.1;
  const goUpIndex = [0, 1, 2],
    goLeftIndex = [0, 3, 6],
    goRightIndex = [2, 5, 8],
    goDownIndex = [6, 7, 8];
  gsap.to(secondSectionDivs, {
    scale: 1 + 2.5 * progress,
    filter: `brightness(${1 - 0.5 * progress})`,
  });
  gsap.to(".secondSectionMainImg", {
    backgroundSize: 25 + 75 * progress + "%",
  });
  for (const index in secondSectionDivs) {
    gsap.to(secondSectionDivs[index], {
      ...(goUpIndex.includes(Number(index)) && {
        y: -translateY + "px",
      }),
      ...(goDownIndex.includes(Number(index)) && {
        y: translateY + "px",
      }),
      ...(goLeftIndex.includes(Number(index)) && {
        x: -translateX + "px",
      }),
      ...(goRightIndex.includes(Number(index)) && {
        x: translateX + "px",
      }),
    });
  }
};

onMounted(() => {
  gsap.registerPlugin(ScrollTrigger, Flip);
  thirdSectionImgsAdd();
  const secondSectionDivs =
    document.querySelectorAll(".secondSection div") || [];
  const thirdSectionImgArr =
    document.querySelectorAll(".thirdSection .item img") || [];
  gsap.set([".firstSectionMainImg", ...secondSectionDivs], {
    filter: "brightness(1)",
  });
  secondSectionDataObj = {
    width:
      document.querySelector<HTMLElement>(".secondSectionMainImg")
        ?.offsetWidth || 0,
    height:
      document.querySelector<HTMLElement>(".secondSectionMainImg")
        ?.offsetHeight || 0,
  };

  //SECTION 1
  gsap.to(".firstSectionMainImg", {
    width: window.innerWidth,
    height: window.innerHeight,
    filter: "brightness(0.5)",
    scrollTrigger: {
      trigger: ".firstSection",
      start: "center center",
      end: "3000 center",
      toggleActions: "restart none reverse none",
      pin: true,
      scrub: 0,
    },
    onComplete: () => {
      gsap.to(".firstSectionText", {
        yPercent: -100,
      });
    },
  });

  Flip.fit(".secondSectionNeededToFit", ".secondSectionMoveTo", {
    duration: 10,
    ease: "power1.inOut",
    scale: true,
    fitChild: ".secondSectionMainImg",
    scrollTrigger: {
      trigger: ".secondSection",
      start: "center center",
      end: "4000 center",
      toggleActions: "restart none reverse none",
      pin: true,
      scrub: 0,
    },
    onComplete: () => {
      gsap.to(".secondSectionText", {
        y: -window.innerHeight / 2 + "px",
        yPercent: -100,
      });
    },
  });

  //SECTION 3
  const thirdSectionItemState = Flip.getState(thirdSectionImgArr);
  for (const img of thirdSectionImgArr) {
    document.querySelector(".thirdSectionMain")?.appendChild(img);
  }
  Flip.from(thirdSectionItemState, {
    paused: true,
    absolute: true,
  });
  gsap.to(thirdSectionImgArr, {
    x: 0,
    y: 0,
    width: "300px",
    height: "500px",
    stagger: {
      grid: "auto",
      each: 0.1,
      from: "start",
    },
    scrollTrigger: {
      trigger: ".thirdSection",
      start: "center center",
      end: "12000 center",
      toggleActions: "restart none reverse none",
      pin: true,
      scrub: 0,
    },
    onComplete: () => {
      gsap.to(".thirdSectionText", {
        yPercent: -100,
      });
    },
  });

  //SECTION 4
  const fourthSectionImgArr =
    document.querySelectorAll(".fourthSection .item img") || [];
  const fourthSectionText = document.querySelector(
    ".fourthSection .fourthSectionText p"
  );
  const fourthSectionItemState = Flip.getState(fourthSectionImgArr);
  const fourthSectionTextState = Flip.getState(fourthSectionText!);

  for (let i = 0; i < fourthSectionImgArr.length; i++) {
    document
      ?.querySelectorAll(".fourthSection .item")[0]
      .appendChild(fourthSectionImgArr[i]);
    gsap.set(fourthSectionImgArr[i], {
      zIndex: fourthSectionImgArr.length - i,
      filter: "brightness(1)",
    });
  }
  document
    ?.querySelectorAll(".fourthSection .item")[0]
    ?.appendChild(fourthSectionText!);
  Flip.from(fourthSectionItemState, {
    paused: true,
    absolute: true,
  });
  Flip.from(fourthSectionTextState, {
    paused: true,
    absolute: true,
  });

  const fourthSectionTimeline = gsap.timeline({
    scrollTrigger: {
      trigger: ".fourthSection",
      start: "center center",
      end: "5000 center",
      toggleActions: "restart none reverse none",
      pin: true,
      scrub: 0,
    },
  });

  for (let i = 0; i < fourthSectionImgArr.length; i++) {
    fourthSectionTimeline.to(
      fourthSectionImgArr[i],
      {
        x: i * 32,
        filter: `brightness(${1 - i * 0.1})`,
      },
      "<"
    );
  }
  fourthSectionTimeline.to(
    fourthSectionText!,
    {
      x: 800,
    },
    "<"
  );

  //SECTION 5
  const fifthSectionImgArr =
    document.querySelectorAll(".fifthSection .item img") || [];
  const fifthSectionText = document.querySelector(
    ".fifthSection .fifthSectionText p"
  );
  const fifthSectionItemState = Flip.getState(fifthSectionImgArr);
  const fifthSectionTextState = Flip.getState(fifthSectionText!);

  for (let i = 0; i < fifthSectionImgArr.length; i++) {
    document
      ?.querySelectorAll(".fifthSection .item")[0]
      .appendChild(fifthSectionImgArr[i]);
    gsap.set(fifthSectionImgArr[i], {
      zIndex: i,
    });
  }
  document
    ?.querySelectorAll(".fifthSection .item")[0]
    ?.appendChild(fifthSectionText!);
  Flip.from(fifthSectionItemState, {
    paused: true,
    absolute: true,
  });
  Flip.from(fifthSectionTextState, {
    paused: true,
    absolute: true,
  });

  const fifthSectionTimeline = gsap.timeline({
    scrollTrigger: {
      trigger: ".fifthSection",
      start: "center center",
      end: "5000 center",
      toggleActions: "restart none reverse none",
      pin: true,
      scrub: 0,
    },
  });

  for (let i = 0; i < fifthSectionImgArr.length; i++) {
    fifthSectionTimeline.to(
      fifthSectionImgArr[i],
      {
        x: i * 32,
        opacity: 1 - i * 0.1,
      },
      "<"
    );
  }
  fifthSectionTimeline.to(
    fifthSectionText!,
    {
      x: 800,
    },
    "<"
  );

  //SECTION 6
  const sixthSectionImgArr =
    document.querySelectorAll(".sixthSection .item img") || [];
  const sixthSectionText = document.querySelector(
    ".sixthSection .sixthSectionText p"
  );
  const sixthSectionItemState = Flip.getState(sixthSectionImgArr);
  const sixthSectionTextState = Flip.getState(sixthSectionText!);

  for (let i = 0; i < sixthSectionImgArr.length; i++) {
    document
      ?.querySelectorAll(".sixthSection .item")[0]
      .appendChild(sixthSectionImgArr[i]);
    gsap.set(sixthSectionImgArr[i], {
      zIndex: sixthSectionImgArr.length - i,
      scale: 1,
      filter: "brightness(1)",
    });
  }
  document
    ?.querySelectorAll(".sixthSection .item")[0]
    ?.appendChild(sixthSectionText!);
  Flip.from(sixthSectionItemState, {
    paused: true,
    absolute: true,
  });
  Flip.from(sixthSectionTextState, {
    paused: true,
    absolute: true,
  });

  const sixthSectionTimeline = gsap.timeline({
    scrollTrigger: {
      trigger: ".sixthSection",
      start: "center center",
      end: "5000 center",
      toggleActions: "restart none reverse none",
      pin: true,
      scrub: 0,
    },
  });

  for (let i = 0; i < sixthSectionImgArr.length; i++) {
    sixthSectionTimeline.to(
      sixthSectionImgArr[i],
      {
        x: i * 32,
        scale: 1 - i * 0.02,
        filter: `brightness(${1 - i * 0.1})`,
      },
      "<"
    );
  }
  sixthSectionTimeline.to(
    sixthSectionText!,
    {
      x: 800,
    },
    "<"
  );

  //SECTION 7
  gsap.set(".seventhSection .sBackground", {
    scale: 3,
    filter: "grayscale(1)",
  });
  gsap.to(".seventhSection .sBackground", {
    scale: 1,
    filter: "grayscale(0)",
    scrollTrigger: {
      trigger: ".seventhSection",
      start: "center center",
      end: "5000 center",
      toggleActions: "reverse none restart none",
      pin: true,
      scrub: 0,
    },
  });
});
</script>
