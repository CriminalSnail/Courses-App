<script  setup >

import { ref } from 'vue'


var show = ref(false)
var faq = ref('closed')
const apear = (question) => {
  if (show.value == false) {
    show.value = true
    console.log(show)
    faq.value = question
    console.log(faq.value)
  } else {
    faq.value = 'closed'
    show.value = false
    console.log(show.value, faq.value)
  }
}



  


</script>

<template>
  <section class="p-20 xl:p-[100px] mx-24 xl:mx-40 mt-[100px]">
    <div style="grid-template-columns: 1fr 2fr" class="grid gap-20 xl:gap-[120px] justify-between">
      <section>
        <header class="flex flex-col gap-10 xl:gap-[50px]">
          <div class="flex flex-col gap-2">
            <h1 class="text-[38px]/[46px] xl:text-[48px]/[56px] font-semibold">Frequently Asked Questions</h1>
            <p class="text-base xl:text-lg/[27px]">
              Still you have any questions? Contact our Team via support@skillbridge.com
            </p>
          </div>
          <div class="flex justify-start">
            <div class="px-5 py-3.5 xl:px-[24px] xl:py-[18px] text-lg "><a>See All FAQ’s</a></div>
          </div>
        </header>
      </section>

      <section class="flex flex-col gap-7">
        <div class="flex flex-col gap-10 p-10">
          <section class="flex justify-between question">
            <p class="text-lg xl:text-xl flex leading-7 items-center">
              Can I enroll in multiple courses at once?
            </p>
            <button
              @click="
                () => {
                  apear(`first`)
                }
              "
              class="p-2.5 bgg-yellow rounded-md"
            >
              <img v-show=" faq != 'first'" src="../assets/icons/plus-sign.svg" />
              <img v-show=" faq === 'first'" src="../assets/icons/close-back-icon.svg" />
             
            </button>
          </section>

          <transition-group name="answer" appear>
            <section
              v-show="show == true && faq == `first`"
              key="answer"
              class="flex justify-between"
            >
              <p class="text-base xl:text-[18px] gray-font flex items-center">
                Absolutely! You can enroll in multiple courses simultaneously and access them at
                your convenience.
              </p>
            </section>

            <section
              v-show="show == true && faq == `first`"
              key="link"
              class="flex justify-between px-10 py-6"
            >
              <p class="text-base flex dark-gray items-center px-6 py-4">
                Enrollment Process for Different Courses
              </p>
              <button class="p-2.5 rounded-md">
                <img src="../assets/icons/faq-arrow.svg" />
              </button>
            </section>
          </transition-group>
        </div>

        <div class="flex flex-col gap-10 px-10 py-6  xl:px-[50px] xl:py-[30px]">
          <section class="flex justify-between question" key="question2">
            <p class="text-lg xl:text-xl/[30px]  flex items-center">
              What kind of support can I expect from instructors?
            </p>
            <div class="p-2.5 bgg-yellow h-11 w-11 rounded-md">
              <button
                @click="
                  () => {
                    apear(`second`)
                  }
                "
                class="bgg-yellow rounded-md"
              >
                <img
                  v-show=" faq != 'second'"
                  src="../assets/icons/plus-sign.svg"
                />

                <img
                  v-show=" faq == 'second'"
                  src="../assets/icons/close-back-icon.svg"
                />
                
              </button>
            </div>
          </section>

          <transition-group name="answer" appear>
            <section
              v-show="show  && faq == `second`"
              key="answer"
              class="flex justify-between"
            >
              <p class="text-base xl:text-[18px] gray-font flex items-center">
                We work to make youre learning process as easy as possible, thats why our instructors will guide you through all difficulties thet may arise in the process.
              </p>
            </section>

            
          </transition-group>

          
        </div>

        <div class="flex flex-col gap-10 px-10 py-6  xl:px-[50px] xl:py-[30px]">
          <section class="flex justify-between question">
            <p class="text-lg xl:text-xl/[30px] flex items-center">
              Are the courses self-paced or do they have specific start and end dates?
            </p>
            <div @click=" () => {apear('third')}" class="p-2.5 bgg-yellow h-11 rounded-md">
              <img   v-show=" faq != 'third'" src="../assets/icons/plus-sign.svg" />
              <img   v-show=" faq == 'third'" src="../assets/icons/close-back-icon.svg" />
            </div>
          </section>

          <transition-group name="answer" appear>
            <section
              v-show="show  && faq == `third`"
              key="answer"
              class="flex justify-between"
            >
              <p class="text-base xl:text-[18px] gray-font flex items-center">
               We designed our courses so you can learn within a group of students like you under a guidense of a experiensed instructor, thats why our courses have start  and  finish date. Althogh most of the materials of the courses leave the pase of complition up to you.    
              </p>
            </section>

            
          </transition-group>
        </div>

        <div class="flex flex-col gap-10 px-10 py-6  xl:px-[50px] xl:py-[30px]">
          <section class="flex justify-between question">
            <p class="text-lg xl:text-xl flex items-center">Are there any prerequisites for the courses?</p>
            <div @click=" () => {apear('fourth')}" class="p-2.5 bgg-yellow h-11 rounded-md">
              <img   v-show=" faq != 'fourth'" src="../assets/icons/plus-sign.svg" />
              <img   v-show=" faq == 'fourth'" src="../assets/icons/close-back-icon.svg" />
            </div>
          </section>





          <transition-group name="answer" appear>
            <section
              v-show="show  && faq == `fourth`"
              key="answer"
              class="flex justify-between"
            >
              <p class="text-base xl:text-[18px] gray-font flex items-center">
              In some cases yes, our couses designed for more advanced.
              </p>
            </section>

            
          </transition-group>
        </div>

        <div class="flex flex-col gap-10 px-10 py-6  xl:px-[50px] xl:py-[30px]">
          <section class="flex justify-between question">
            <p class="text-lg xl:text-xl/[30px] flex items-center">
              Can I download the course materials for offline access?
            </p>
            <div @click=" () => {apear('fifth')}" class="p-2.5 bgg-yellow h-11 rounded-md">
              <img   v-show=" faq != 'fifth'" src="../assets/icons/plus-sign.svg" />
              <img   v-show=" faq == 'fifth'" src="../assets/icons/close-back-icon.svg" />
            </div>
          </section>


          <transition-group name="answer" appear>
            <section
              v-show="show  && faq == `fifth`"
              key="answer"
              class="flex justify-between"
            >
              <p class="text-base xl:text-[18px] gray-font flex items-center">
              Shure, all of the videos and streams are avalible for download and accsessible online.
              </p>
            </section>

            
          </transition-group>
        </div>

       
      </section>
    </div>
  </section>
</template>
