<template>
<div>
  <div x-data="{ open: false }" class="relative bg-white overflow-hidden">
    <div class="max-w-screen-xl mx-auto ">
      <div class="relative z-10 pb-8 bg-white sm:pb-16 md:pb-20 lg:max-w-2xl lg:w-full lg:pb-28 xl:pb-32">
        <div class="pt-6 px-4 sm:px-6 lg:px-8">
          <nav class="relative flex items-center justify-between sm:h-10 lg:justify-start">
            <div class="flex items-center flex-grow flex-shrink-0 lg:flex-grow-0">
              <div class="flex items-center justify-between w-full md:w-auto">
                <a href="#">
                  <img class="h-8 w-auto sm:h-10" src="/images/logo.png" alt="" />
                </a>
                <div class="-mr-2 flex items-center md:hidden">
                  <button @click="open = true" type="button" class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:bg-gray-100 focus:text-gray-500 transition duration-150 ease-in-out">
                    <svg class="h-6 w-6" stroke="currentColor" fill="none" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                    </svg>
                  </button>
                </div>
              </div>
            </div>
            <div class="hidden md:block md:ml-10 md:pr-4">
              <a href="#equipe" class="font-medium text-gray-500 hover:text-gray-900 focus:outline-none focus:text-gray-900 transition duration-150 ease-in-out">Equipe</a>
              <a href="#" class="ml-8 font-medium text-gray-500 hover:text-gray-900 focus:outline-none focus:text-gray-900 transition duration-150 ease-in-out">Horaires</a>
              <a href="#" class="ml-8 font-medium text-gray-500 hover:text-gray-900 focus:outline-none focus:text-gray-900 transition duration-150 ease-in-out">Soins</a>
              <a href="#cabinet" class="ml-8 font-medium text-gray-500 hover:text-gray-900 focus:outline-none focus:text-gray-900 transition duration-150 ease-in-out">Cabinet</a>
            </div>
          </nav>
        </div>

        <div x-show="open" x-transition:enter="duration-150 ease-out" x-transition:enter-start="opacity-0 scale-95" x-transition:enter-end="opacity-100 scale-100" x-transition:leave="duration-100 ease-in" x-transition:leave-start="opacity-100 scale-100" x-transition:leave-end="opacity-0 scale-95" class="absolute top-0 inset-x-0 p-2 transition transform origin-top-right md:hidden">
          <div class="rounded-lg shadow-md">
            <div class="rounded-lg bg-white shadow-xs overflow-hidden">
              <div class="px-5 pt-4 flex items-center justify-between">
                <div>
                  <img class="h-8 w-auto" src="/images/logo.png" alt="logo" />
                </div>
                <div class="-mr-2">
                  <button @click="open = false" type="button" class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:bg-gray-100 focus:text-gray-500 transition duration-150 ease-in-out">
                    <svg class="h-6 w-6" stroke="currentColor" fill="none" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
                    </svg>
                  </button>
                </div>
              </div>
              <div class="px-2 pt-2 pb-3">
                <a href="#equipe" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out">Equipe</a>
                <a href="#" class="mt-1 block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out">Horaires</a>
                <a href="#" class="mt-1 block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out">Soins</a>
                <a href="#cabinet" class="mt-1 block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out">Cabinet</a>
              </div>
              <div>
                <a href="#" class="block w-full px-5 py-3 text-center font-medium text-indigo-600 bg-gray-50 hover:bg-gray-100 hover:text-indigo-700 focus:outline-none focus:bg-gray-100 focus:text-indigo-700 transition duration-150 ease-in-out">
                  Log in
                </a>
              </div>
            </div>
          </div>
        </div>

        <div class="mt-10 mx-auto max-w-screen-xl px-4 sm:mt-12 sm:px-6 md:mt-16 lg:mt-20 lg:px-8 xl:mt-28">
          <div class="sm:text-center lg:text-left">
            <h2 class="text-4xl tracking-tight leading-10 font-extrabold text-gray-900 sm:text-5xl sm:leading-none md:text-6xl">
              Data to enrich your
              <br class="xl:hidden" />
              <span class="text-indigo-600">online business</span>
            </h2>
            <p class="mt-3 text-base text-gray-500 sm:mt-5 sm:text-lg sm:max-w-xl sm:mx-auto md:mt-5 md:text-xl lg:mx-0">
              Anim aute id magna aliqua ad ad non deserunt sunt. Qui irure qui lorem cupidatat commodo. Elit sunt amet fugiat veniam occaecat fugiat aliqua.
            </p>

            <div class="lg:flex lg:items-center lg:justify-between">
              <div class="flex-1 min-w-0">
                <div class="mt-1 flex flex-col sm:mt-0 sm:flex-row sm:flex-wrap">
                  <div class="mt-2 flex items-center text-sm leading-5 text-gray-500 sm:mr-6">
                    <svg class="flex-shrink-0 mr-1.5 h-5 w-5 text-gray-400" fill="currentColor" viewBox="0 0 20 20">
                      <path fill-rule="evenodd" d="M5.05 4.05a7 7 0 119.9 9.9L10 18.9l-4.95-4.95a7 7 0 010-9.9zM10 11a2 2 0 100-4 2 2 0 000 4z" clip-rule="evenodd"/>
                    </svg>
                    93 rue de paris, 94220 Charenton-le-pont
                  </div>
                  <div class="mt-2 flex items-center text-sm leading-5 text-gray-500">
                    <svg class="flex-shrink-0 mr-1.5 h-5 w-5 text-gray-400" fill="currentColor" viewBox="0 0 20 20">
                      <path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"/>
                    </svg>
                    Tous les jours 6h - 20h
                  </div>
                </div>
              </div>
            </div>

            <div class="mt-5 sm:mt-8 sm:flex sm:justify-center lg:justify-start">
              <div class="rounded-md shadow">
                <a href="#" class="w-full flex items-center justify-center px-8 py-3 border border-transparent text-base leading-6 font-medium rounded-md text-white bg-green-600 hover:bg-green-700 focus:outline-none focus:shadow-outline transition duration-150 ease-in-out md:py-4 md:text-lg md:px-10">
                  <svg class="fill-current w-4 h-4 mr-2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20">
                  <path d="M20 18.35V19a1 1 0 0 1-1 1h-2A17 17 0 0 1 0 3V1a1 1 0 0 1 1-1h4a1 1 0 0 1 1 1v4c0 .56-.31 1.31-.7 1.7L3.16 8.84c1.52 3.6 4.4 6.48 8 8l2.12-2.12c.4-.4 1.15-.71 1.7-.71H19a1 1 0 0 1 .99 1v3.35z"/></svg>
                  <span>01 43 53 37 44</span>
                </a>
              </div>
              <div class="mt-3 sm:mt-0 sm:ml-3">
                <a href="#" class="w-full flex items-center justify-center px-8 py-3 border border-transparent text-base leading-6 font-medium rounded-md text-green-700 border-green-400 hover:text-green-600 hover:bg-green-100 focus:outline-none focus:shadow-outline focus:border-indigo-300 transition duration-150 ease-in-out md:py-4 md:text-lg md:px-10">
                  <svg class="fill-current w-4 h-4 mr-2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M1 4c0-1.1.9-2 2-2h14a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2V4zm2 2v12h14V6H3zm2-6h2v2H5V0zm8 0h2v2h-2V0zM5 9h2v2H5V9zm0 4h2v2H5v-2zm4-4h2v2H9V9zm0 4h2v2H9v-2zm4-4h2v2h-2V9zm0 4h2v2h-2v-2z"/></svg>
                  <span>En ligne</span>
                </a>
              </div>
            </div>
          </div>
        </div>
        <svg class="hidden lg:block absolute right-0 inset-y-0 h-full w-48 text-white transform translate-x-1/2" fill="currentColor" viewBox="0 0 100 100" preserveAspectRatio="none">
          <polygon points="50,0 100,0 50,100 0,100" />
        </svg>
      </div>
    </div>
    <div class="lg:absolute lg:inset-y-0 lg:right-0 lg:w-1/2">
      <img class="h-56 w-full object-cover sm:h-72 md:h-96 lg:w-full lg:h-full"
      src="/images/bg.jpg"
      alt="" />
    </div>
  </div>

  <!-- equipe -->
  <div class="bg-gray-200 p-4">
    <h2 id="equipe" class="text-indigo-600 text-2xl font-semibold">Equipe</h2>
    <div class="flex flex-row justify-center">
      <div class="px-4 py-2 m-2">
        <img class="" src="/images/ninie-min.jpg" alt="" />
        <p class="text-lg font-medium">Annie-Caroline</p>
        <p class="text-mg font-medium">MONSEAU</p>
        <p>diplomé bla bla bla</p>
      </div>
      <div class="px-4 py-2 m-2">
        <img class="" src="/images/bab-min.jpg" alt="" />
        <p class="text-lg font-medium">Marie-Elisabeth</p>
        <p class="text-mg font-medium">MATHUREL</p>
        <p>diplomé bla bla bla</p>
      </div>
    </div>
  </div>


  <!-- cabinet -->
  <div class="bg-gray-900 p-4">
    <h2 id="cabinet" class="text-indigo-600 text-2xl font-semibold">Cabinet</h2>
    <div class="flex flex-row justify-center">
      <div class="px-4 py-2 m-2">
        <img class="" src="/images/cab1.jpg" alt="" />
      </div>
      <div class="px-4 py-2 m-2">
        <img class="" src="/images/cab2.jpg" alt="" />
      </div>
    </div>
  </div>

  <!-- soins -->
<div>
  <h2 id="soins" class="text-indigo-600 text-2xl font-semibold">soins</h2>
  <div class="flex flex-row justify-center">
      <div class="px-4 py-2 m-2">
        <h3>Injections</h3>
        <img class="w-8" src="/images/soins/plaster.png" alt="" />
        <ul>
          <li>sous-cunaté</li>
          <li>intraveineuse</li>
        </ul>
      </div>

     <div class="px-4 py-2 m-2">
        <h3>Pansements</h3>
        <img class="w-8" src="/images/soins/syringe.png" alt="" />
        <ul>
          <li>sous-cunaté</li>
          <li>intraveineuse</li>
        </ul>
      </div>

    </div>
</div>


</div>
</template>