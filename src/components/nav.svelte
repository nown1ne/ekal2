<script>
    import icon from '$lib/assets/auriga.png';
    let open = false;
    let handle = () => {open = !open;}
    import {slide} from 'svelte/transition'
    let links = ["Suggestions","Report","Videocon","Contact"]
</script>

{#if open}
<div transition:slide class="sitkcy z-50 top-0 h-screen w-screen  py-20 bg-gray-900">
  <button on:click={handle} data-collapse-toggle="navbar-cta" type="button" class="float-right p-2 text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="navbar-cta" aria-expanded="false">
    <span class="sr-only">Open main menu</span>
    <svg class="w-6 h-6" aria-hidden="true" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z" clip-rule="evenodd"></path></svg>
</button>
<div class="grid-col-1  p-5 my-10 container mx-auto">
  {#each links as link}
  <div class="px-8 py-2 mx-auto container text-center text-4xl my-20 text-gray-100 trasnform hover:scale-120" transition:slide on:click={handle}><a href="/{link}" class="">{link}</a></div>
  {/each}
</div>
</div>
{/if}
<nav class=" border-gray-200 shadow-md dark:shadow-lg py-3.5 bg-gray-900 sticky top-0 z-50">
    <div class="container flex flex-wrap justify-between items-center mx-auto">
    <a href="/" class="flex items-center transform hover:scale-125"> 
        <img src={icon} class="shadow-lg dark:shadow-none mr-3 h-10 sm:h-9 md:h-11" alt="Auriga Logo">
    </a>
    <div class="flex md:order-2">
        <button  type="button" class="text-white bg-blue-700 hover:bg-blue-800  focus:outline-none gfont-medium rounded-lg text-sm px-8 py-3.5 text-center mr-3 md:mr-0 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">Login</button>
        <button on:click={handle} data-collapse-toggle="navbar-cta" type="button" class="inline-flex items-center p-2 text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="navbar-cta" aria-expanded="false">
          <span class="sr-only">Open main menu</span>
          <svg class="w-6 h-6" aria-hidden="true" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z" clip-rule="evenodd"></path></svg>
      </button>
    </div>
    <div class="p-2 hidden justify-between items-center w-full md:flex md:w-auto md:order-1" id="navbar-cta">
      <ul class="flex flex-col p-4 mt-4  rounded-lg border md:flex-row md:space-x-8 md:mt-0 md:text-sm md:font-medium md:border-0 bg-gray-800 dark:bg-gray-900 border-gray-700">
        <li>
          <a href="/Suggestions" class="transform hover:scale-110 text-xl block py-2 pr-4 pl-3 rounded   md:p-0 md:hover:text-white text-gray-400 hover:bg-gray-700 hover:text-white md:hover:bg-transparent border-gray-700">Suggestions</a>
        </li>
        <li>
          <a href="" class="transform hover:scale-110 text-xl block py-2 pr-4 pl-3 rounded   md:p-0 md:hover:text-white text-gray-400 hover:bg-gray-700 hover:text-white md:hover:bg-transparent border-gray-700" >Report Analysis</a>
        </li>
        <li>
          <a href="#" class="transform hover:scale-110 text-xl block py-2 pr-4 pl-3 rounded   md:p-0 md:hover:text-white text-gray-400 hover:bg-gray-700 hover:text-white md:hover:bg-transparent border-gray-700">Video Conferencing</a>
        </li>
        <li>
          <a href="/Contact" class="transform hover:scale-110 text-xl block py-2 pr-4 pl-3 rounded   md:p-0 md:hover:text-white text-gray-400 hover:bg-gray-700 hover:text-white md:hover:bg-transparent border-gray-700">Contact Us</a>
        </li>
      </ul>
    </div>
    </div>
  </nav>


  