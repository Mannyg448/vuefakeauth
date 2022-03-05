<script setup>
import useAuth from "../composable/useAuth";
const {isAuthenticated, logout} = useAuth();
</script>



<template>
   <div class="bg-pink-300 text-gray-500">
        <div class="container mx-auto flex items-center italic justify-between ">
            <h1 class="tracking-tighter text-3xl font-semibold">
                Vue<span class="font-normal">FakeAuth</span>
                </h1>
            <nav>
                <ul class="flex space-x-4">
                    <router-link to="/">
                    <li class="py-8 px-4  hover:cursor-pointer hover:bg-gray-500 hover:text-pink-300">
                        Home
                        </li></router-link>
                     <router-link to="/about">   
                    <li class="py-8 px-4 hover:cursor-pointer hover:bg-gray-500 hover:text-pink-300">About</li>
                    </router-link>
                    <router-link v-if="!isAuthenticated" to="/login">
                    <li class="py-8 px-4 hover:cursor-pointer hover:bg-gray-500 hover:text-pink-300">Login</li>
                    </router-link>

                    <div v-else class="flex">
                     <router-link  to="/secret">
                    <li class="py-8 px-4 hover:cursor-pointer hover:bg-gray-500 hover:text-pink-300">Secret</li>
                    </router-link>


                     <button  @click="logout">
                    <li class="py-8 px-4 hover:cursor-pointer hover:bg-gray-500 hover:text-pink-300">Logout</li>
                    </button>
                    </div>
                    
                </ul>

            </nav>
        </div>
        </div>
    
</template>