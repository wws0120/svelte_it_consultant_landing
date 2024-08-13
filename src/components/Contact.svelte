<script>
  import SectionWrapper from './SectionWrapper.svelte';
  import {
    IconMapPin,
    IconPhoneCall,
    IconClock,
    IconUser,
    IconMail,
    IconPhone,
    IconBuilding,
    IconMessage,
  } from '@tabler/icons-svelte';
</script>

<section id="contact" class=" bg-gradient-to-b from-teal-50/80 to-green-50/80">
  <SectionWrapper>
    <div class="container mx-auto">
      <div class="relative z-10 lg:flex lg:gap-10">
        <div class="lg:w-1/2 p-10 text-gray-800">
          <p class="mt-4 text-sm leading-7 font-semibold uppercase">Contact</p>
          <h3
            class="text-3xl sm:text-4xl text-gray-800 leading-normal font-extrabold tracking-tight"
          >
            Get In <span class="text-teal-600">Touch</span>
          </h3>
          <p class="mt-4 mb-8 text-gray-800 leading-7">
            We combine cutting-edge technology with industry expertise to
            deliver results that drive growth and efficiency. Contact us today
            to learn how we can support your digital transformation journey.
          </p>

          <div class="flex items-center mt-5">
            <IconMapPin size={28} class="text-teal-600 mr-2" />
            <span class="text-sm font-semibold"
              >Room 1002, Street 12, Lorem Road, Ipsum, Some Country.</span
            >
          </div>
          <div class="flex items-center mt-5">
            <IconPhoneCall size={28} class="text-teal-600 mr-2" />
            <span class="text-sm font-semibold">+00 123 45 67 89</span>
          </div>
          <div class="flex items-center mt-5">
            <IconClock size={28} class="text-teal-600 mr-2" />
            <span class="text-sm font-semibold"
              >Mon to Fri from 9 a.m. to 5 p.m.</span
            >
          </div>
        </div>
        <form
          action=""
          class="rounded-3xl bg-white px-4 py-12 lg:w-1/2 lg:px-8"
        >
          <div class="grid gap-10 sm:grid-cols-2">
            <div class="relative">
              <input
                type="text"
                name="name"
                class="w-full rounded-2xl border-2 border-gray/20 bg-transparent p-4 font-bold outline-none transition focus:border-secondary ltr:pr-12 rtl:pl-12"
              />
              <label
                for=""
                class="absolute -top-3 bg-white px-2 font-bold left-6"
                >Full Name</label
              >
              <IconUser
                class="absolute top-1/2 -translate-y-1/2 right-4"
                stroke={2}
              />
            </div>
            <div class="relative">
              <input
                type="email"
                name="email"
                class="w-full rounded-2xl border-2 border-gray/20 bg-transparent p-4 font-bold outline-none transition focus:border-secondary ltr:pr-12 rtl:pl-12"
              />
              <label
                for=""
                class="absolute -top-3 bg-white px-2 font-bold left-6"
                >Email Address</label
              >
              <IconMail
                class="absolute top-1/2 -translate-y-1/2 right-4"
                stroke={2}
              />
            </div>
            <div class="relative">
              <input
                type="text"
                name="mobile"
                class="w-full rounded-2xl border-2 border-gray/20 bg-transparent p-4 font-bold outline-none transition focus:border-secondary ltr:pr-12 rtl:pl-12"
              />
              <label
                for=""
                class="absolute -top-3 bg-white px-2 font-bold left-6"
                >Mobile Number</label
              >
              <IconPhone
                class="absolute top-1/2 -translate-y-1/2 right-4"
                stroke={2}
              />
            </div>
            <div class="relative">
              <input
                type="text"
                name="city"
                class="w-full rounded-2xl border-2 border-gray/20 bg-transparent p-4 font-bold outline-none transition focus:border-secondary ltr:pr-12 rtl:pl-12"
              />
              <label
                for=""
                class="absolute -top-3 bg-white px-2 font-bold left-6"
                >City</label
              >
              <IconBuilding
                class="absolute top-1/2 -translate-y-1/2 right-4"
                stroke={2}
              />
            </div>
          </div>
          <div class="relative mt-10">
            <input
              type="text"
              name="message"
              class="w-full rounded-2xl border-2 border-gray/20 bg-transparent p-4 font-bold outline-none transition focus:border-secondary ltr:pr-12 rtl:pl-12"
            />
            <label for="" class="absolute -top-3 bg-white px-2 font-bold left-6"
              >Message</label
            >
            <IconMessage
              class="absolute top-1/2 -translate-y-1/2 right-4"
              stroke={2}
            />
          </div>
          <div class="mt-10 text-center ltr:lg:text-right rtl:lg:text-left">
            <button
              type="button"
              class="btn bg-gray px-12 capitalize text-white"
            >
              Send Message
            </button>
          </div>
        </form>
      </div>
    </div>
  </SectionWrapper>
</section>
