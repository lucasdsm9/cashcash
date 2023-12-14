<template>
    
    
    <div class="flex min-h-screen">

      <nav class="flex w-full bg-gray-200 h-28">
        Lucas DSM
      </nav>
      <!-- sidebar -->
      <div class="sidebar bg-gray-200 h-screen fixed w-[300px] p-4">
        
        <div class="flex items-center justify-center">
          <img src="@/assets/logo.png" class="w-28" alt="logo cashcash">
        </div>
        
      <div>
        <ul class="flex flex-col text-xl justify-start">
            
              <router-link to="/">
                <li :class="{ 'text-white bg-[#3241B3]': $route.path === '/' }" class="mt-5 py-[6px] hover:text-white hover:bg-[#3241B3] w-full text-center rounded-lg">
                  Dashboard
                </li>
              </router-link>
            
              <router-link to="/client"><font-awesome-icon :icon="['fas', 'user-group']" style="color: #000000;"/> 
                <li :class="{ 'text-white bg-[#3241B3]': $route.path === '/client' }" class="mt-1 py-[6px] hover:text-white hover:bg-[#3241B3] w-full text-center rounded-lg">
                  Clients
                </li>
              </router-link>

              <router-link to="/statistique">
                <li :class="{ 'text-white bg-[#3241B3]': $route.path === '/statistique' }" class="mt-1 py-[6px] hover:text-white hover:bg-[#3241B3] w-full text-center rounded-lg">
                  Statistiques
                </li>
              </router-link>
            
              <router-link to="/intervention">
                <li :class="{ 'text-white bg-[#3241B3]': $route.path === '/intervention' }" class="mt-1 py-[6px] hover:text-white hover:bg-[#3241B3] w-full text-center rounded-lg">
                  Interventions
                </li>
              </router-link>

              <router-link to="/technicien">
                <li :class="{ 'text-white bg-[#3241B3]': $route.path === '/technicien' }" class=" mt-1 py-[6px] hover:text-white hover:bg-[#3241B3] w-full text-center rounded-lg">
                  Techniciens
                </li>
              </router-link>
        </ul>
      </div>

      </div>
  
      <!-- main -->
      <main>
        <router-view />
      </main>
    </div>



  </template>
  
  