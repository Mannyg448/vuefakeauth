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
                    <router-link to="/login">
                    <li class="py-8 px-4 hover:cursor-pointer hover:bg-gray-500 hover:text-pink-300">Hello</li>
                    </router-link>

                     <router-link to="/us">
                    <li class="py-8 px-4 hover:cursor-pointer hover:bg-gray-500 hover:text-pink-300">Us</li>
                    </router-link>
                    
                </ul>

            </nav>
        </div>
        </div>
    
</template>