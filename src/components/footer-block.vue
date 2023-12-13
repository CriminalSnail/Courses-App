<template>
          <section class="flex flex-col gap-14 xl:gap-[100px] px-[80px] pt-[60px] pb-[20px] xl:px-[162px] xl:pt-[100px] ">
        <div class="flex justify-between">
          <section class="flex flex-col w-1/5 gap-[30px] xl:gap-[40px]">
            <section>
              <div class="xl:p-[7px] p-[5.7px]">
                <img
                  class="bg-cont rounded-md xl:w-[40px] xl:h-[40px] w-[32.5px] h-[32.5px]"
                  src="../assets/icons/product-icon.svg"
                  alt=""
                  srcset=""
                />
              </div>
            </section>

            <section class="flex flex-col gap-3.5 ">
              <div class="flex gap-1 xl:gap-[6px]">
                <img class="w-[20px] h-[20px] xl:w-[24px] xl:h-[24px]" src="../assets/icons/mail-icon.svg" />
                <a class="text-lg">hello@skillbridge.com</a>
              </div>
              <div class="flex gap-1 xl:gap-[6px]">
                <img class="w-[20px] h-[20px] xl:w-[24px] xl:h-[24px]" src="../assets/icons/phone-icon.svg" />
                <a class="text-lg">+91 91813 23 2309</a>
              </div>
              <div class="flex gap-1 xl:gap-[6px]">
                <img class="w-[20px] h-[20px] xl:w-[24px] xl:h-[24px]" src="../assets/icons/location-icon.svg" />
                <a class="text-lg">Somewhere in the World</a>
              </div>
            </section>
          </section>

          <nav class="flex w-3/5 gap-6 xl:gap-[30px]">
            <section class="flex flex-col flex-auto w-33 gap-2.5">
              <div><h1 class="text-lg xl:text-xl font-semibold">Home</h1></div>

              <div class="flex flex-col gap-2">
                <div><a class="lightest-gray-font text-base xl:text-lg"> Benefits</a></div>
                <div><a class="lightest-gray-font text-base xl:text-lg">Our Courses</a></div>
                <div><a class="lightest-gray-font text-base xl:text-lg"> Our Testimonials</a></div>
                <div><a class="lightest-gray-font text-base xl:text-lg">Our FAQ</a></div>
              </div>
            </section>

            <section class="flex flex-col flex-auto w-33 gap-2.5">
              <div><h1 class="text-lg xl:text-xl font-semibold">About</h1></div>

              <section class="flex flex-col gap-2">
                <div><a class="lightest-gray-font text-base xl:text-lg"> Company</a></div>
                <div><a class="lightest-gray-font text-base xl:text-lg">Achievements</a></div>
                <div><a class="lightest-gray-font text-base xl:text-lg"> Our Goals</a></div>
              </section>
            </section>

            <section class="flex flex-col flex-auto w-33 gap-2.5">
              <div><h1 class="text-lg xl:text-xl font-semibold">Social Profiles</h1></div>

              <section class="flex gap-3.5 ">
                <div class="p-[12px] xl:p-3.5">
                  <a class="lightest-gray-font ">
                    <img class="w-5 h-5 xl:w-6 xl:h-6" src="../assets/icons/facebook-icon.svg"
                  /></a>
                </div>
                <div class="p-[12px] xl:p-3.5">
                  <a class="lightest-gray-font"
                    ><img class="w-5 h-5 xl:w-6 xl:h-6" src="../assets/icons/twitter-icon.svg"
                  /></a>
                </div>
                <div class="p-[12px] xl:p-3.5">
                  <a class="lightest-gray-font"
                    ><img class="w-5 h-5 xl:w-6 xl:h-6" src="../assets/icons/linkedin-icon.svg"
                  /></a>
                </div>
              </section>
            </section>
          </nav>
        </div>

        <section class="flex justify-center">
          <p class="text-lg">© 2023 Skillbridge. All rights reserved.</p>
        </section>
      </section>
</template>


<script>
 export default {
    data() {
      return {
        
      };
    }
  };



</script>