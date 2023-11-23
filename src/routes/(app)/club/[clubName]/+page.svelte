<script>
    import pomi from "$lib/assets/images/pomi.png";
    import Modal from './Modal.svelte';

    let showModal = false;
    let introduce = "";
    $: introduce;

</script>

<section>

    <div class="h-screen px-4 pb-24 overflow-auto md:px-6">
        <div class="flex h-10 w-3/4 justify-between my-3">
            <div class="flex items-start text-3xl mb-4 font-semibold text-gray-800 dark:text-white">
                동호회 신청
            </div>
            <button type="button" on:click={() => (showModal = true)} class="py-1 px-3 flex justify-center items-center bg-purple-500 hover:bg-purple-700 focus:ring-purple-500 focus:ring-offset-purple-200 text-white transition ease-in duration-200 text-center text-base font-semibold shadow-md focus:outline-none focus:ring-2 focus:ring-offset-2  rounded-lg ">
                <svg width="20" height="20" fill="currentColor" class="mr-2" viewBox="0 0 1792 1792" xmlns="http://www.w3.org/2000/svg">
                    <path d="M1344 1472q0-26-19-45t-45-19-45 19-19 45 19 45 45 19 45-19 19-45zm256 0q0-26-19-45t-45-19-45 19-19 45 19 45 45 19 45-19 19-45zm128-224v320q0 40-28 68t-68 28h-1472q-40 0-68-28t-28-68v-320q0-40 28-68t68-28h427q21 56 70.5 92t110.5 36h256q61 0 110.5-36t70.5-92h427q40 0 68 28t28 68zm-325-648q-17 40-59 40h-256v448q0 26-19 45t-45 19h-256q-26 0-45-19t-19-45v-448h-256q-42 0-59-40-17-39 14-69l448-448q18-19 45-19t45 19l448 448q31 30 14 69z">
                    </path>
                </svg>
                신청
            </button>
        </div>
        <div class="w-3/4 mb-4 overflow-hidden shadow-lg rounded-2xl">
            <div class="relative w-full p-4 bg-white">
                <img alt="eggs" src="{pomi}"/>
                <hr class="my-4"/>
                <p class="mb-2 text-2xl font-semibold border-b w-max text-gray-800">
                    곰인형 동호회
                </p>
                <p class="text-gray-600">
                    서울특별시 중구
                </p>
                <div class="flex flex-wrap items-center mt-3 justify-starts">
                    <div class="text-xs mb-2 mr-2 py-1.5 px-3 text-gray-600 bg-pink-100 rounded-2xl">
                        #곰인형
                    </div>
                    <div class="text-xs mb-2 mr-2 py-1.5 px-3 text-gray-600 bg-pink-100 rounded-2xl">
                        #귀여운것
                    </div>
                </div>
            </div>
        </div>
        <div class="w-3/4 mb-4 overflow-hidden shadow-lg rounded-2xl h-90">
            <div class="relative w-full p-4 bg-white">
                <p class="font-bold text-xl mb-3 text-gray-700 border-b border-gray-200 w-max dark:text-white">
                    동호회 소개
                </p>
                <div class="">
                    우리는 귀여운 곰인형을 사랑하는 사람들이 모여서 함께 인형놀이를 하는 귀여운 동호회입니다.
                </div>
            </div>
        </div>

        <div class="w-3/4 mb-4 overflow-hidden shadow-lg rounded-2xl h-90">
            <div class="relative w-full p-4 bg-white">
                <p class="font-bold text-xl mb-3 text-gray-700 border-b border-gray-200 w-max dark:text-white">
                    동호회 정보
                </p>
                <div class="flex flex-col my-3">
                    <div class="flex items-center">
                        <span class="relative p-3 bg-yellow-300 rounded-full">
                            <svg width="20" height="20" fill="currentColor" viewBox="0 0 2304 1792" class="absolute h-3 text-gray-700 transform -translate-x-1/2 -translate-y-1/2 left-1/2 top-1/2" xmlns="http://www.w3.org/2000/svg">
                                <path d="M1728 448l-384 704h768zm-1280 0l-384 704h768zm821-192q-14 40-45.5 71.5t-71.5 45.5v1291h608q14 0 23 9t9 23v64q0 14-9 23t-23 9h-1344q-14 0-23-9t-9-23v-64q0-14 9-23t23-9h608v-1291q-40-14-71.5-45.5t-45.5-71.5h-491q-14 0-23-9t-9-23v-64q0-14 9-23t23-9h491q21-57 70-92.5t111-35.5 111 35.5 70 92.5h491q14 0 23 9t9 23v64q0 14-9 23t-23 9h-491zm-181 16q33 0 56.5-23.5t23.5-56.5-23.5-56.5-56.5-23.5-56.5 23.5-23.5 56.5 23.5 56.5 56.5 23.5zm1088 880q0 73-46.5 131t-117.5 91-144.5 49.5-139.5 16.5-139.5-16.5-144.5-49.5-117.5-91-46.5-131q0-11 35-81t92-174.5 107-195.5 102-184 56-100q18-33 56-33t56 33q4 7 56 100t102 184 107 195.5 92 174.5 35 81zm-1280 0q0 73-46.5 131t-117.5 91-144.5 49.5-139.5 16.5-139.5-16.5-144.5-49.5-117.5-91-46.5-131q0-11 35-81t92-174.5 107-195.5 102-184 56-100q18-33 56-33t56 33q4 7 56 100t102 184 107 195.5 92 174.5 35 81z">
                                </path>
                            </svg>
                        </span>
                        <p class="ml-2 text-gray-700 text-md font-semibold dark:text-gray-50">
                            동호회장
                        </p>
                    </div>
                    <div class="flex flex-col justify-start">
                        <p class="my-2 ml-1 text-xl font-bold text-left text-gray-800 dark:text-white">
                            박지현
                        </p>
                    </div>
                </div>
                <div class="flex flex-col my-3">
                    <div class="flex items-center">
                        <span class="relative p-3 bg-purple-300 rounded-full">
                            <svg width="20" height="20" class="absolute h-3 text-purple-500 transform -translate-x-1/2 -translate-y-1/2 top-1/2 left-1/2" viewBox="0 0 1792 1792" xmlns="http://www.w3.org/2000/svg">
                                <path d="M1664 960q-152-236-381-353 61 104 61 225 0 185-131.5 316.5t-316.5 131.5-316.5-131.5-131.5-316.5q0-121 61-225-229 117-381 353 133 205 333.5 326.5t434.5 121.5 434.5-121.5 333.5-326.5zm-720-384q0-20-14-34t-34-14q-125 0-214.5 89.5t-89.5 214.5q0 20 14 34t34 14 34-14 14-34q0-86 61-147t147-61q20 0 34-14t14-34zm848 384q0 34-20 69-140 230-376.5 368.5t-499.5 138.5-499.5-139-376.5-368q-20-35-20-69t20-69q140-229 376.5-368t499.5-139 499.5 139 376.5 368q20 35 20 69z">
                                </path>
                            </svg>
                        </span>
                        <p class="ml-2 text-gray-700 text-md font-semibold dark:text-gray-50">
                            회원수
                        </p>
                    </div>
                    <div class="flex flex-col justify-start">
                        <p class="my-2 ml-1 text-xl font-bold text-left text-gray-800 dark:text-white">
                            13명
                        </p>
                    </div>
                </div>
                <div class="flex items-center">
                    <span class="relative p-3 bg-green-200 rounded-full">
                        <svg width="20" fill="currentColor" height="20" class="absolute h-4 text-purple-500 transform -translate-x-1/2 -translate-y-1/2 top-1/2 left-1/2" viewBox="0 0 1792 1792" xmlns="http://www.w3.org/2000/svg">
                            <path d="M1362 1185q0 153-99.5 263.5t-258.5 136.5v175q0 14-9 23t-23 9h-135q-13 0-22.5-9.5t-9.5-22.5v-175q-66-9-127.5-31t-101.5-44.5-74-48-46.5-37.5-17.5-18q-17-21-2-41l103-135q7-10 23-12 15-2 24 9l2 2q113 99 243 125 37 8 74 8 81 0 142.5-43t61.5-122q0-28-15-53t-33.5-42-58.5-37.5-66-32-80-32.5q-39-16-61.5-25t-61.5-26.5-62.5-31-56.5-35.5-53.5-42.5-43.5-49-35.5-58-21-66.5-8.5-78q0-138 98-242t255-134v-180q0-13 9.5-22.5t22.5-9.5h135q14 0 23 9t9 23v176q57 6 110.5 23t87 33.5 63.5 37.5 39 29 15 14q17 18 5 38l-81 146q-8 15-23 16-14 3-27-7-3-3-14.5-12t-39-26.5-58.5-32-74.5-26-85.5-11.5q-95 0-155 43t-60 111q0 26 8.5 48t29.5 41.5 39.5 33 56 31 60.5 27 70 27.5q53 20 81 31.5t76 35 75.5 42.5 62 50 53 63.5 31.5 76.5 13 94z">
                            </path>
                        </svg>
                    </span>
                    <p class="ml-2 text-gray-700 text-md font-semibold dark:text-gray-50">
                        회비
                    </p>
                </div>
                <div class="flex flex-col justify-start">
                    <p class="my-2 ml-1 text-xl font-bold text-left text-gray-700 dark:text-gray-100">
                        20,000원
                    </p>
                </div>
            </div>
        </div>
    </div>

    <Modal bind:showModal>
        <div class="my-1 text-lg font-semibold" slot="header">
            자기 소개를 입력해주세요!
        </div>

        <textarea class="text-sm rounded-xl p-1" cols="50" rows="10" placeholder="자기소개를 입력해주세요" bind:value={introduce}></textarea>
    </Modal>
</section>



<style>
</style>
