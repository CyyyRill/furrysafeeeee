<template>
    <section class="mx-[5rem] py-32">
    <div class="overflow-hidden border-b border-muted">
      <div class="container">
        <div class="mx-auto flex max-w-5xl flex-col items-center">
          <div class="z-10 items-center text-center">
            <h1 class="mb-8 text-pretty text-4xl font-medium lg:text-8xl">
                Make Every Day a Perfect Pet Day
            </h1>
            <p class="mx-auto max-w-screen-md text-zinc-600 lg:text-xl">
              Discover a world of fun and care for your furry friends. From grooming to playtime, we’ve got everything to make tails wag! Explore now
            </p>
            <div class="mt-12 flex w-full flex-col justify-center gap-2 sm:flex-row">
              <button
                class="inline-flex items-center justify-center whitespace-nowrap rounded-md text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 bg-zinc-900 text-white hover:bg-zinc-900/90 h-10 px-4 py-2">
                Get started now<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"
                  fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
                  class="lucide lucide-chevron-right ml-2 h-4">
                  <path d="m9 18 6-6-6-6"></path>
                </svg></button><button
                class="inline-flex items-center justify-center whitespace-nowrap rounded-md text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 hover:bg-zinc-100 hover:text-zinc-800 h-10 px-4 py-2">
                Learn more<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
                  stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
                  class="lucide lucide-chevron-right ml-2 h-4">
                  <path d="m9 18 6-6-6-6"></path>
                </svg>
              </button>
            </div>
          </div>
        </div>
        <img :src="require('@/assets/images/Photo-350-1920x1080-e19366e.jpg')" alt="placeholder"
          class="mx-auto mt-24 max-h-[700px] w-full max-w-7xl rounded-t-lg object-cover shadow-lg" />
      </div>
    </div>
  </section>
  
  <section class="bg-[#f8f8f8] py-16 px-4">
      <div class="max-w-6xl mx-auto">
        <!-- Headers -->
        <div class="text-center mb-16">
          <h2 class="text-gray-600 mb-4">The challenge</h2>
          <h3 class="text-4xl  text-gray-800">All pets deserve Love. We help them find it.</h3>
        </div>
  
        <!-- Statistics Grid -->
        <div class="z-10 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
          <!-- Stat 1 -->
          <div class="text-center">
            <div class="w-16 h-16 mx-auto mb-4 bg-gray-100 rounded-full flex items-center justify-center">
              <svg class="w-8 h-8 text-black-600" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M3 9L12 2L21 9V20C21 20.5304 20.7893 21.0391 20.4142 21.4142C20.0391 21.7893 19.5304 22 19 22H5C4.46957 22 3.96086 21.7893 3.58579 21.4142C3.21071 21.0391 3 20.5304 3 20V9Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M9 22V12H15V22" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
            </div>
            <h4 class="text-black-600 text-2xl font-medium mb-2">1 million+ pets</h4>
            <p class="text-gray-600">never find a loving home.</p>
          </div>
  
          <!-- Stat 2 -->
          <div class="text-center">
            <div class="w-16 h-16 mx-auto mb-4 bg-gray-100 rounded-full flex items-center justify-center">
              <svg class="w-8 h-8 text-black-600" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M20.84 4.61a5.5 5.5 0 0 0-7.78 0L12 5.67l-1.06-1.06a5.5 5.5 0 0 0-7.78 7.78l1.06 1.06L12 21.23l7.78-7.78 1.06-1.06a5.5 5.5 0 0 0 0-7.78z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
            </div>
            <h4 class="text-black-600 text-2xl font-medium mb-2">Many</h4>
            <p class="text-gray-600">pets are unnecessarily euthanized without accessible veterinary care.</p>
          </div>
  
          <!-- Stat 3 -->
          <div class="text-center">
            <div class="w-16 h-16 mx-auto mb-4 bg-gray-100 rounded-full flex items-center justify-center">
              <svg class="w-8 h-8 text-black-600" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M11 19C15.4183 19 19 15.4183 19 11C19 6.58172 15.4183 3 11 3C6.58172 3 3 6.58172 3 11C3 15.4183 6.58172 19 11 19Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M21 21L16.65 16.65" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
            </div>
            <h4 class="text-black-600 text-2xl font-medium mb-2">1 in 3</h4>
            <p class="text-gray-600">pets go missing and many never make it back home.</p>
          </div>
  
          <!-- Stat 4 -->
          <div class="text-center">
            <div class="w-16 h-16 mx-auto mb-4 bg-gray-100 rounded-full flex items-center justify-center">
              <svg class="w-8 h-8 text-black-600" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <circle cx="12" cy="12" r="10" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M16 8H15.3C14.5 8 14 8.5 13.7 9.1L11.3 14.9C11 15.5 10.5 16 9.7 16H9C8.2 16 7.7 15.5 7.4 14.9L5 9.1C4.7 8.5 4.2 8 3.4 8" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
            </div>
            <h4 class="text-black-600 text-2xl font-medium mb-2">Countless</h4>
            <p class="text-gray-600">shelters and organizations are under resourced.</p>
          </div>
        </div>
      </div>
    </section>
  
  <section class="py-32 mx-10">
    <div class="grid items-center gap-10 lg:grid-cols-2 lg:gap-20">
      <div class="flex justify-end bg-zinc-100">
        <img :src="require('@/assets/images/sleeping-dogs.jpeg')" alt="placeholder hero"
          class="max-h-[600px] w-full rounded-md object-cover lg:max-h-[800px]" />
      </div>
      <div class="flex flex-col items-center text-center lg:max-w-3xl lg:items-start lg:text-left">
        
        <h1 class="my-6 text-pretty text-4xl font-bold lg:text-4xl xl:text-5xl">
         Committed to people, pets and the planet
        </h1>
        <p class="mb-8 max-w-xl text-zinc-600 lg:text-2xl">
          We're prioritising the happiness of animals and reducing our environmental impact through pet caring and home sharing.
        </p>
        <div class="flex w-full flex-col justify-center gap-2 sm:flex-row lg:justify-start">
          <button
            class="inline-flex items-center justify-center whitespace-nowrap rounded-md text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 bg-zinc-900 text-white hover:bg-zinc-900/90 h-10 px-4 py-2 w-full sm:w-auto">
            Start now</button>
        </div>
      </div>
    </div>
  </section>
  
  <section class="py-32 mx-10">
    <div class="grid items-center gap-10 lg:grid-cols-2 lg:gap-20">   
      <div class="flex flex-col items-center text-center lg:max-w-3xl lg:items-start lg:text-left">
        
        <h1 class="my-6 text-pretty text-4xl font-bold lg:text-4xl xl:text-5xl">
          Home is where the heart is 
        </h1>
        <p class="mb-8 max-w-xl text-zinc-600 lg:text-2xl">
          When you can’t be there, remember that your pets got Peeps!
        Make sure your pet gets the care and attention they deserve when you’re away at work or on holiday.
        </p>
        <div class="flex w-full flex-col justify-center gap-2 sm:flex-row lg:justify-start">
          <button
            class="inline-flex items-center justify-center whitespace-nowrap rounded-md text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 border border-input bg-white hover:bg-zinc-100 hover:text-zinc-800 h-10 px-4 py-2 w-full sm:w-auto">
            Login now<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
              stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
              class="lucide lucide-arrow-down-right ml-2 size-4">
              <path d="m7 7 10 10"></path>
              <path d="M17 7v10H7"></path>
            </svg>
          </button>
        </div>
      </div>
      <div class="flex justify-end bg-zinc-100">
        <img :src="require('@/assets/images/young-smiling-happy-cheerful-owner-600nw-2397244269.webp')" alt="placeholder hero"
          class="max-h-[600px] w-full rounded-md object-cover lg:max-h-[800px]" />
      </div>
    </div>
  </section>
  
  <section class="py-32 mx-10">
    <div class="container">
      <div class="mx-auto grid max-w-screen-lg gap-10 md:grid-cols-2">
        <div class="order-1 flex flex-col gap-2 rounded-lg border p-2">
          <img :src="require('@/assets/images/images (1).jpg')" alt="placeholder"
            class="aspect-video w-full rounded-lg border object-cover" />
          <div data-orientation="horizontal" role="none" class="shrink-0 bg-border h-[1px] w-full"></div>
          <img :src="require('@/assets/images/images.jpg')" alt="placeholder"
            class="aspect-video w-full rounded-lg border object-cover" />
        </div>
        <div class="order-3 rounded-lg border p-2">
          <img :src="require('@/assets/images/photo_2023-04-03-23_05_46-300x300.jpeg')" alt="placeholder"
            class="h-full w-full rounded-lg border object-cover" />
        </div>
        <div class="order-2 -mt-6 max-w-[412px] md:order-3">
          <p class="mb-6 text-sm text-zinc-600 md:mb-12">Animal Week</p>
          <h3 class="mb-3 text-2xl font-medium md:mb-6">National Animal Shelter Week</h3>
          <p class="mb-6">
            National Animal Shelter Week is a celebration of animal shelters and the staff who work tirelessly to support animals and the people who love them.    
          </p>
          <a href="#" class="font-medium hover:underline">Learn more about our process</a>
        </div>
        <div class="order-4 -mt-6 max-w-[412px] md:order-3">
          <p class="mb-6 text-sm text-zinc-600 md:mb-12">Heartwarming adoption stories </p>
          <h3 class="mb-3 text-2xl font-medium md:mb-6">Heartwarming adoption stories from 2024 to inspire you</h3>
          <p class="mb-6">
            Adoption adds so much to your life — joy, excitement, companionship — but it also changes the life of an animal forever. At Animal Humane Society, we love giving animals a second chance to find a loving family, and we encourage every adopter to share their stories with us.
          </p>
          <a href="#" class="font-medium hover:underline">Learn more about our process</a>
        </div>
      </div>
    </div>
  </section>
  
  
  
  <section class="py-32 mx-10">
    <div class="container flex flex-col items-center text-center">
      <h2 class="my-6 text-pretty text-2xl font-bold lg:text-4xl">Meet our team</h2>
      <p class="mb-8 max-w-3xl text-zinc-600 lg:text-xl">
        We’re a passionate team dedicated to delivering exceptional solutions. Meet the people behind our innovative work!
      </p>
    </div>
    <div class="container mt-16 grid gap-x-8 gap-y-16 md:grid-cols-2 lg:grid-cols-4">
      <div class="flex flex-col items-center">
        <img :src="require('@/assets/images/467339479_3822145781436016_8671856640929245081_n.jpg')"
          class="relative flex shrink-0 overflow-hidden rounded-full mb-4 size-20 border md:mb-5 lg:size-24" />
        <p class="text-center font-medium">Jennifer Quiza</p>
        <p class="text-center text-zinc-600">Backend</p>
      </div>
      <div class="flex flex-col items-center">
        <img :src="require('@/assets/images/466489064_2357506981250141_2387006246628246180_n.jpg')"
          class="relative flex shrink-0 overflow-hidden rounded-full mb-4 size-20 border md:mb-5 lg:size-24" />
        <p class="text-center font-medium">Marijoe Gotong</p>
        <p class="text-center text-zinc-600">Frontend</p>
      </div>
      <div class="flex flex-col items-center">
        <img :src="require('@/assets/images/461037919_2123111208085786_2188055552214296559_n.jpg')"
          class="relative flex shrink-0 overflow-hidden rounded-full mb-4 size-20 border md:mb-5 lg:size-24" />
        <p class="text-center font-medium">June Cyril Dolendo</p>
        <p class="text-center text-zinc-600">Frontend</p>
      </div>
      <div class="flex flex-col items-center">
        <img :src="require('@/assets/images/467311469_1301549980840895_3946468965201337037_n.jpg')"
          class="relative flex shrink-0 overflow-hidden rounded-full mb-4 size-20 border md:mb-5 lg:size-24" />
        <p class="text-center font-medium">Francis Caleb Fabila</p>
        <p class="text-center text-zinc-600">Document</p>
      </div>
      <div class="flex flex-col items-center">
        <img :src="require('@/assets/images/448780448_2168835226882726_6933289752106432956_n.jpg')"
          class="relative flex shrink-0 overflow-hidden rounded-full mb-4 size-20 border md:mb-5 lg:size-24" />
        <p class="text-center font-medium">Leopoldo Salpocial</p>
        <p class="text-center text-zinc-600">Backend</p>
      </div>
      
    </div>
  </section>
  
  <section>
    <div class="relative w-full h-[20rem] overflow-hidden">
      <!-- Video Background -->
      <video 
        class="absolute top-0 left-0 w-full h-full object-cover"
        autoplay 
        muted 
        loop 
        playsinline
      >
        <source src="https://videos.ctfassets.net/gynu23gx3hnw/3TcnKUPCircPk3raaa1kh9/64c4cf3de068c13b610c4d7eeb3ab102/Web_looping_video_5_sec_compressed.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      
      <!-- Dark Overlay -->
      <div class="absolute inset-0 bg-black/30"></div>
      
      <!-- Content -->
      <div class="relative h-full flex flex-col items-center justify-center text-center px-4">
        <h1 class="text-3xl md:text-6xl lg:text-3xl text-white font-serif mb-4">
          <span class="font-normal">Got</span>
          <span class="font-medium"> Love</span>
          <span class="font-normal">? Give</span>
          <span class="font-medium"> Love.</span>
        </h1>
        
        <button 
          class="mt-8 px-8 py-3 text-white border-2 border-white rounded-full 
                 hover:bg-white hover:text-black transition-colors duration-300
                 text-lg font-medium"
          @click="handleDonate"
        >
          Donate
        </button>
      </div>
    </div>
  </section>
  <section class="py-5 mx-11">
    <div class="container">
      <footer>
        <div class="flex flex-col justify-between gap-4 md:flex-row md:items-center">   
        </div>
        <div data-orientation="horizontal" role="none" class="shrink-0 bg-border h-[1px] w-full my-14"></div>
        <div class="grid gap-8 md:grid-cols-2 lg:grid-cols-4">
          <div>
            <h3 class="mb-4 font-bold">Product</h3>
            <ul class="space-y-4 text-zinc-600">
              <li class="font-medium hover:text-gray-800"><a href="#">Overview</a></li>
              <li class="font-medium hover:text-gray-800"><a href="#">Pricing</a></li>
              <li class="font-medium hover:text-gray-800"><a href="#">Marketplace</a></li>
              <li class="font-medium hover:text-gray-800"><a href="#">Features</a></li>
              <li class="font-medium hover:text-gray-800"><a href="#">Integrations</a></li>
              <li class="font-medium hover:text-gray-800"><a href="#">Pricing</a></li>
            </ul>
          </div>
          <div>
            <h3 class="mb-4 font-bold">Company</h3>
            <ul class="space-y-4 text-zinc-600">
              <li class="font-medium hover:text-gray-800"><a href="#">About</a></li>
              <li class="font-medium hover:text-gray-800"><a href="#">Team</a></li>
              <li class="font-medium hover:text-gray-800"><a href="#">Blog</a></li>
              <li class="font-medium hover:text-gray-800"><a href="#">Careers</a></li>
              <li class="font-medium hover:text-gray-800"><a href="#">Contact</a></li>
              <li class="font-medium hover:text-gray-800"><a href="#">Privacy</a></li>
            </ul>
          </div>
          <div>
            <h3 class="mb-4 font-bold">Resources</h3>
            <ul class="space-y-4 text-zinc-600">
              <li class="font-medium hover:text-gray-800"><a href="#">Help</a></li>
              <li class="font-medium hover:text-gray-800"><a href="#">Sales</a></li>
              <li class="font-medium hover:text-gray-800"><a href="#">Advertise</a></li>
            </ul>
          </div>
          <div>
            <h3 class="mb-4 font-bold">Legal</h3>
            <ul class="space-y-4 text-zinc-600">
              <li class="font-medium hover:text-gray-800"><a href="#">Term of Services</a></li>
              <li class="font-medium hover:text-gray-800"><a href="#">Privacy Policy</a></li>
            </ul>     
          </div>
        </div>
        <div data-orientation="horizontal" role="none" class="shrink-0 bg-border h-[1px] w-full my-14"></div>
      </footer>
    </div>
  </section>
  
  
  
  </template>
  
  <script>
  export default {
    name: "UserHome",
    data() {
      return {
        posts: [
          {
            id: 1,
            username: "user1",
            profile: "profile1.jpg",
            image: "post1.jpg",
            caption: "Beautiful day!",
            likes: 1234,
            comments: 56,
            time: "2 HOURS AGO"
          },
          // ... more posts
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  
  h1 {
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);}
  
  
  
  </style>