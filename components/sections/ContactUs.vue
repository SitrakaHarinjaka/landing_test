<template>
  <section id="contact" class="mt-[180px] mb-[102px]">
    <div class="title-section text-center mb-20">
       <h3 class="text-titleSection">Contact us</h3>
       <p class="text-secondText">Most calendars are designed for teams. Slate is designed for freelancers</p>
    </div>
    <div class="container">
       <div class="contact-container">
          <div class="formulaire flex gap-10">
             <form action="" class="flex flex-col w-1/3 bg-white border border-[#DDDDDD] shadow-[0px_13px_19px_rgba(0,0,0,0.07)] rounded-[20px] p-[52px_50px]">
                <h4 class="text-[20px] leading-[28px] tracking-[0.1px] font-bold mb-[3px] text-[#252B42] text-center mb-7">Contact Us</h4>

                <input type="text" name="Your name" id="" placeholder="Your name" class="mb-10">
                <input type="email" name="Your email" id="" placeholder="Your email" class="mb-10">
                <textarea name="message" id="" class="mb-10 resize-none" rows="12">Your message</textarea>

                <div class="btn-container">
                  <input type="submit" value="Send" class="button-primary">
                </div>

             </form>

             <div class="contact-content w-2/3 flex flex-col gap-12">
                <div class="location flex items-center">
                  <div class="text-center address w-1/3 flex items-center flex-col">
                    <div>
                      <LocalisationIcon/>
                    </div>
                    <p class="text-secondText py-7">
                      6386 Spring St undefined Anchorage, Georgia 12473 United States
                    </p>
                  </div>
                  <div class="text-center phone w-1/3 flex items-center flex-col">
                    <div>
                      <PhoneIcon/>
                    </div>
                    <p class="text-secondText py-7">(843) 555-0130</p>
                  </div>
                  <div class="text-center mail w-1/3 flex items-center flex-col">
                    <div>
                      <EnvelopIcon/>
                    </div>
                    <p class="text-secondText py-7">willie.jennings@example.com</p>
                  </div>
                </div>

                <div class="map self-center">
                  <img src="~/assets/img/@ map screen.png" alt="">
                </div>

                <div class="socials flex">
                  <div class="mr-3">
                    <svg
                      width="34"
                      height="28"
                      viewBox="0 0 34 28"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M33.6455 4.0808C32.4207 4.60914 31.0878 4.98939 29.7149 5.13749C31.1403 4.29068 32.2077 2.95287 32.7168 1.37505C31.3793 2.17072 29.914 2.72866 28.386 3.02412C27.7474 2.34138 26.975 1.79748 26.117 1.42631C25.2589 1.05514 24.3337 0.864651 23.3988 0.866716C19.6163 0.866716 16.5744 3.93271 16.5744 7.69515C16.5744 8.22349 16.6384 8.75183 16.7425 9.26016C11.0788 8.96397 6.02753 6.25821 2.66936 2.11553C2.05746 3.16067 1.7368 4.35068 1.74075 5.56176C1.74075 7.9313 2.94553 10.0207 4.78273 11.2495C3.70004 11.2068 2.64271 10.9092 1.69672 10.3809V10.4649C1.69672 13.7831 4.04225 16.5329 7.16827 17.1653C6.58133 17.3178 5.97753 17.3957 5.37111 17.3974C4.92682 17.3974 4.50655 17.3534 4.08227 17.2934C4.94683 19.9991 7.46447 21.9644 10.4624 22.0284C8.11689 23.8656 5.17898 24.9463 1.98891 24.9463C1.41654 24.9463 0.8882 24.9263 0.339844 24.8623C3.36581 26.8035 6.95614 27.9243 10.8226 27.9243C23.3748 27.9243 30.2432 17.5255 30.2432 8.49967C30.2432 8.20348 30.2432 7.90728 30.2232 7.61109C31.5521 6.63846 32.7168 5.43368 33.6455 4.0808Z"
                        fill="#2091F9"
                      />
                    </svg>
                  </div>
        
                  <div class="mr-3">
                    <svg
                      width="33"
                      height="33"
                      viewBox="0 0 33 33"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M31.7126 0.385254H2.25349C1.54503 0.385254 0.972656 0.957625 0.972656 1.66609V31.1252C0.972656 31.8337 1.54503 32.406 2.25349 32.406H31.7126C32.4211 32.406 32.9934 31.8337 32.9934 31.1252V1.66609C32.9934 0.957625 32.4211 0.385254 31.7126 0.385254ZM28.0142 9.73132H25.4565C23.4512 9.73132 23.063 10.6839 23.063 12.0848V15.1708H27.8501L27.2257 20.002H23.063V32.406H18.0718V20.006H13.897V15.1708H18.0718V11.6085C18.0718 7.47385 20.5974 5.22039 24.2878 5.22039C26.0569 5.22039 27.5739 5.35248 28.0182 5.41252V9.73132H28.0142Z"
                        fill="#2091F9"
                      />
                    </svg>
                  </div>
        
                  <div class="mr-3">
                    <svg
                      width="33"
                      height="33"
                      viewBox="0 0 33 33"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M31.697 0.385254H2.23786C1.5294 0.385254 0.957031 0.957625 0.957031 1.66609V31.1252C0.957031 31.8337 1.5294 32.406 2.23786 32.406H31.697C32.4054 32.406 32.9778 31.8337 32.9778 31.1252V1.66609C32.9778 0.957625 32.4054 0.385254 31.697 0.385254ZM10.4552 27.671H5.70411V12.389H10.4552V27.671ZM8.08165 10.2997C7.53701 10.2997 7.00459 10.1382 6.55173 9.83559C6.09887 9.533 5.74591 9.10292 5.53749 8.59973C5.32906 8.09654 5.27453 7.54285 5.38078 7.00866C5.48704 6.47448 5.74931 5.9838 6.13443 5.59868C6.51956 5.21355 7.01023 4.95128 7.54442 4.84503C8.0786 4.73877 8.63229 4.7933 9.13548 5.00173C9.63867 5.21016 10.0688 5.56312 10.3713 6.01598C10.6739 6.46884 10.8354 7.00125 10.8354 7.5459C10.8314 9.06689 9.59864 10.2997 8.08165 10.2997ZM28.2427 27.671H23.4957V20.2381C23.4957 18.465 23.4636 16.1875 21.0261 16.1875C18.5565 16.1875 18.1762 18.1168 18.1762 20.1101V27.671H13.4331V12.389H17.9881V14.4784H18.0521C18.6845 13.2776 20.2335 12.0088 22.547 12.0088C27.3582 12.0088 28.2427 15.1748 28.2427 19.2895V27.671Z"
                        fill="#2091F9"
                      />
                    </svg>
                  </div>
                </div>
             </div>
          </div>
       </div>
    </div>
 </section>
</template>

<script lang="ts" setup>
import LocalisationIcon from '~/assets/svg/LocalisationIcon.svg'
import PhoneIcon from "~/assets/svg/PhoneIcon.svg"
import EnvelopIcon from "~/assets/svg/EnvelopIcon.svg"

</script>

<style>

</style>