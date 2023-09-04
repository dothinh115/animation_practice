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
                <div class="flex justify-center items-center gap-8" ref="firstSection">
                    <div class="min-w-[123px] h-[185px] rounded-[6px] overflow-hidden">
                        <img src="/images/1_1.jpg" class="w-full h-full object-cover" />
                    </div>
                    <div class="min-w-[155px] h-[232px] rounded-[6px] overflow-hidden">
                        <img src="/images/1_2.jpg" class="w-full h-full object-cover" />
                    </div>
                    <div class="min-w-[310px] h-[465px] rounded-[6px] overflow-hidden">
                        <img src="/images/1_3.jpg" class="w-full h-full object-cover" />
                    </div>
                    <div class="w-[465px] h-[650px] min-h-[650px] aspect-w-3 aspect-h-5 rounded-[6px] overflow-hidden flex-shrink-0"
                        ref="firstSectionMainImg">
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
                        tantalizing facade, captivating our gaze. Yet, as we search for
                        the soul of human expression, we question whether algorithms can
                        truly embody the essence of authentic art.
                    </p>
                </div>
            </div>
        </section>
        <section class="mt-[500px]">
            <div class="px-16 text-white my-16">
                <h2 class="text-[45px] font-bold tracking-wide">SECTION 2</h2>
            </div>
            <div class="relative">
                <div class="w-screen h-screen grid grid-cols-3 grid-rows-3 gap-x-[calc(2.5vw)] gap-y-[calc(3vh)] overflow-hidden"
                    ref="secondSection">
                    <div class="w-full h-full rounded-[6px] overflow-hidden min-h-fit min-w-fit">
                        <img src="/images/2_1.jpg" class="w-full h-full" />
                    </div>
                    <div class="w-full h-full rounded-[6px] overflow-hidden min-h-fit min-w-fit">
                        <img src="/images/2_2.jpg" class="w-full h-full" />
                    </div>
                    <div class="w-full h-full rounded-[6px] overflow-hidden min-h-fit min-w-fit">
                        <img src="/images/2_3.jpg" class="w-full h-full" />
                    </div>
                    <div class="w-full h-full rounded-[6px] overflow-hidden min-h-fit min-w-fit">
                        <img src="/images/2_4.jpg" class="w-full h-full" />
                    </div>
                    <div class="w-full h-full rounded-[6px] overflow-hidden min-h-fit min-w-fit z-50 bg-[url('/images/2_main.jpg')] bg-cover"
                        ref="secondSectionMainImg">
                    </div>
                    <div class="w-full h-full rounded-[6px] overflow-hidden min-h-fit min-w-fit">
                        <img src="/images/2_5.jpg" class="w-full h-full" />
                    </div>
                    <div class="w-full h-full rounded-[6px] overflow-hidden min-h-fit min-w-fit">
                        <img src="/images/2_6.jpg" class="w-full h-full" />
                    </div>
                    <div class="w-full h-full rounded-[6px] overflow-hidden min-h-fit min-w-fit">
                        <img src="/images/2_7.jpg" class="w-full h-full" />
                    </div>
                    <div class="w-full h-full rounded-[6px] overflow-hidden min-h-fit min-w-fit">
                        <img src="/images/2_8.jpg" class="w-full h-full" />
                    </div>
                </div>
                <div class="px-16 text-white secondSectionText">
                    <p class="text-[20px] font-semibold tracking-wide w-[450px]">
                        Within this meticulously arranged AI-generated ensemble lies a
                        tantalizing facade, captivating our gaze. Yet, as we search for
                        the soul of human expression, we question whether algorithms can
                        truly embody the essence of authentic art.
                    </p>
                </div>
            </div>
        </section>
        <section class="mt-[500px]">
            <div class="px-16 text-white my-16">
                <h2 class="text-[45px] font-bold tracking-wide">SECTION 3</h2>
            </div>
            <div class="relative">
                <div class=" grid grid-cols-10 grid-rows-4 w-screen h-[calc(80vh)] gap-8" v-html="thirdSectionItemsCalc()"
                    ref="thirdSection">
                </div>
                <div class="absolute top-1/2 -translate-y-1/2 left-1/2 -translate-x-1/2 w-[300px] h-[500px]"
                    ref="thirdSectionMain"></div>
            </div>

        </section>
        <section class="h-[5000px]"></section>
    </main>
</template>
<script setup lang="ts">
import { gsap } from "gsap";
import { ScrollTrigger } from "gsap/ScrollTrigger";

const firstSection = ref<HTMLDivElement | null>(null);
const firstSectionMainImg = ref<HTMLDivElement | null>(null);
const secondSection = ref<HTMLDivElement | null>(null);
const secondSectionMainImg = ref<HTMLDivElement | null>(null);
const thirdSection = ref<HTMLDivElement | null>(null);
const thirdSectionMain = ref<HTMLDivElement | null>(null);
let secondSectionDataObj: {
    width: number,
    height: number
}, thirdSectionDataObj: {
    items: number,
    cols: number,
    rows: number,
    mainRectTop: number,
    mainRectLeft: number,
    mainWidth: number,
    mainHeight: number,
    data: {
        node: HTMLElement,
        width: number,
        height: number,
        rectTop: number,
        rectLeft: number,
    }[]
} = {
        items: 16,
        cols: 10,
        rows: 4,
        data: [],
        mainRectTop: 0,
        mainRectLeft: 0,
        mainWidth: 0,
        mainHeight: 0,
    }

const updateSecondSectionPos = (progress: number) => {
    const secondSectionDivs = secondSection.value?.querySelectorAll("div") || [];
    const translateX =
        (window.innerWidth - secondSectionDataObj.width) * progress * 1.1;
    const translateY =
        (window.innerHeight - secondSectionDataObj.height) * progress * 1.1;
    gsap.to(secondSectionDivs, {
        scale: 1 + 2.5 * progress,
        filter: `brightness(${1 - 0.5 * progress})`,
    });
    gsap.to([secondSectionDivs[0], secondSectionDivs[3], secondSectionDivs[6]], {
        x: -translateX + "px",
    });
    gsap.to([secondSectionDivs[2], secondSectionDivs[5], secondSectionDivs[8]], {
        x: translateX + "px",
    });
    gsap.to([secondSectionDivs[0], secondSectionDivs[1], secondSectionDivs[2]], {
        y: -translateY + "px",
    });
    gsap.to([secondSectionDivs[6], secondSectionDivs[7], secondSectionDivs[8]], {
        y: translateY + "px",
    });
    gsap.to(".secondSectionText", {
        y: -window.innerHeight / 2 + "px",
        yPercent: -100,
    });
};

const updateThirdSectionPos = (progress: number) => {
    for (let i = 0; i < thirdSectionDataObj.data.length; i++) {
        const item = thirdSectionDataObj.data[i];
        const xTranslate = (thirdSectionDataObj.mainRectLeft - item.rectLeft) * progress;
        const yTranslate = (thirdSectionDataObj.mainRectTop - item.rectTop) * progress;
        const widthToUpdate = (thirdSectionDataObj.mainWidth - item.width) * progress;
        const heightToUpdate = (thirdSectionDataObj.mainHeight - item.height) * progress;
        gsap.to(item.node, {
            position: 'absolute',
            width: item.width + widthToUpdate,
            height: item.height + heightToUpdate,
            x: xTranslate,
            y: yTranslate,
        })
    }
}

const thirdSectionItemsCalc = (): string => {
    let html = '';
    for (let i = 0; i < thirdSectionDataObj.cols * thirdSectionDataObj.rows; i++) {
        html += `<div class="h-full w-full rounded-[6px] overflow-hidden item"></div>`
    }
    return html;
}

const thirdSectionImgsAdd = () => {
    let posArr: number[] = [];
    const divArr = thirdSection.value?.querySelectorAll(".item") || [];
    for (let i = 0; i < thirdSectionDataObj.items; i++) {
        posArr = [...posArr, i];
    }
    for (const position of posArr) {
        const randomPos = Math.floor(Math.random() * thirdSectionDataObj.cols * thirdSectionDataObj.rows); // 0 - 39
        divArr[randomPos].innerHTML = (`<img src="../images/3_${position + 1}.jpg" class="h-full w-full object-cover rounded-[6px] z-[${randomPos}]" />`);
        posArr = posArr.filter(item => item !== position);
    }

}

onMounted(() => {
    gsap.registerPlugin(ScrollTrigger);
    thirdSectionImgsAdd();
    const secondSectionDivs = secondSection.value?.querySelectorAll("div") || [];
    gsap.set([firstSectionMainImg.value, ...secondSectionDivs], {
        filter: "brightness(1)",
    });
    secondSectionDataObj = {
        width: secondSectionMainImg.value?.offsetWidth || 0,
        height: secondSectionMainImg.value?.offsetHeight || 0,
    }

    const thirdSectionImgArr = thirdSection.value?.querySelectorAll<HTMLElement>(".item img") || [];

    for (const img of thirdSectionImgArr) {
        const node = img;
        const width = img.offsetWidth;
        const height = img.offsetHeight;
        const rectTop = img.getBoundingClientRect().top;
        const rectLeft = img.getBoundingClientRect().left;
        const data = {
            node,
            width,
            height,
            rectTop,
            rectLeft,
        }
        thirdSectionDataObj.data.push(data);
    }

    thirdSectionDataObj.mainRectLeft = thirdSectionMain.value?.getBoundingClientRect().left || 0;
    thirdSectionDataObj.mainRectTop = thirdSectionMain.value?.getBoundingClientRect().top || 0;
    thirdSectionDataObj.mainWidth = thirdSectionMain.value?.offsetWidth || 0;
    thirdSectionDataObj.mainHeight = thirdSectionMain.value?.offsetHeight || 0;

    gsap.to(firstSectionMainImg.value, {
        width: window.innerWidth,
        height: window.innerHeight,
        filter: 'brightness(0.5)',
        scrollTrigger: {
            trigger: firstSection.value,
            start: "center center",
            end: "3000 center",
            toggleActions: "restart none reverse none",
            pin: true,
            scrub: 0
        }
    });

    ScrollTrigger.create({
        trigger: secondSection.value,
        start: "center center",
        end: "3000 center",
        toggleActions: "restart none reverse none",
        pin: true,
        onUpdate: (self: {
            progress: number
        }) => updateSecondSectionPos(self.progress),
    });

    ScrollTrigger.create({
        trigger: thirdSection.value,
        start: "center center",
        end: "3000 center",
        toggleActions: "restart none reverse none",
        pin: true,
        onUpdate: (self: {
            progress: number
        }) => updateThirdSectionPos(self.progress),
    });
})

</script>