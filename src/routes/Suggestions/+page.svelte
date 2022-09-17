<script>
  import Animate from "../../animate.svelte";

</script>
<Animate>
    <main>
        <div class="mt-20 mx-auto  max-w-md container p-20 shadow-md border-1 border-gray-200 rounded-lg mb-20">
            
            <div class="relative">
            <input type="text" id="floating_outlined" class=" bg-transparent block px-2.5 pb-2.5 pt-4 w-full text-sm mb-4 rounded-lg border-2  border-gray-100 appearance-none text-white  focus:outline-none focus:ring-0 focus:border-blue-500 peer" placeholder=" " />
            <label for="floating_outlined" class="absolute text-sm bg-white text-gray-500 duration-300 transform -translate-y-4 scale-75 top-2 z-10 origin-[0]  px-2 peer-focus:px-2 peer-focus:text-blue-500  peer-placeholder-shown:scale-100 peer-placeholder-shown:-translate-y-1/2 peer-placeholder-shown:top-1/2 peer-focus:top-2 peer-focus:scale-75 peer-focus:-translate-y-4 left-1">Suggestion</label>
        </div>
        
    </div>     
</main>
</Animate>