<script>
        import govt from '$lib/assets/gvn.png';
        import edu from '$lib/assets/edu.png';
        import agr from '$lib/assets/agr.png';
        import emp from '$lib/assets/emp.png';
        import serv from '$lib/assets/serv.png';
        import pdv from '$lib/assets/perDev.png';
        import { fade} from "svelte/transition";
</script>

<div class="p-10 pb-20 grid grid-cols-1 gap-4 gap-y-8 md:grid-cols-2 lg:grid-cols-3">

    
<div transition:fade class="hover:shadow-lg mx-auto max-w-sm bg-white rounded-lg border border-gray-200 shadow-md transition-all duration-200 cursor-pointer filter md:saturate-50 hover:saturate-100">
    <a href="">
        <img class="p-3 rounded-t-lg" src={govt} alt="">
    </a>
    <div class="p-5 transition hover:scale-110">
        <a href="">
            <h5 class="mb-2  text-2xl text-center font-bold tracking-tight text-gray-900">Government | सरकार</h5>
        </a>        
    </div>
</div>


<div transition:fade class="hover:shadow-lg mx-auto max-w-sm bg-white rounded-lg border border-gray-200 shadow-md transition-all duration-200 cursor-pointer filter md:saturate-50 hover:saturate-100">
    <a href="">
        <img class="p-3 rounded-t-lg" src={edu} alt="">
    </a>
    <div class="p-5 transition hover:scale-110">
        <a href="">
            <h5 class="mb-2  text-2xl text-center font-bold tracking-tight text-gray-900">Education | शिक्षा</h5>
        </a>        
    </div>
</div>

<div transition:fade class="hover:shadow-lg mx-auto max-w-sm bg-white rounded-lg border border-gray-200 shadow-md transition-all duration-200 cursor-pointer filter md:saturate-50 hover:saturate-100">
    <a href="#">
        <img class="p-3 rounded-t-lg" src={agr} alt="">
    </a>
    <div class="p-5 transition hover:scale-110">
        <a href="#">
            <h5 class="mb-2  text-2xl text-center font-bold tracking-tight text-gray-900">Agriculture | मेरा गाँव</h5>
        </a>        
    </div>
</div>

<div transition:fade class="hover:shadow-lg mx-auto max-w-sm bg-white rounded-lg border border-gray-200 shadow-md transition-all duration-200 cursor-pointer filter md:saturate-50 hover:saturate-100">
    <a href="#">
        <img class="p-3 rounded-t-lg" src={pdv} alt="">
    </a>
    <div class="p-5 transition hover:scale-110">
        <a href="#">
            <h5 class="mb-2  text-2xl text-center font-bold tracking-tight text-gray-900">Personal Development | व्यक्तित्व-विकास</h5>
        </a>        
    </div>
</div>

<div transition:fade class="hover:shadow-lg mx-auto max-w-sm bg-white rounded-lg border border-gray-200 shadow-md transition-all duration-200 cursor-pointer filter md:saturate-50 hover:saturate-100">
    <a href="#">
        <img class="p-3 rounded-t-lg" src={emp} alt="">
    </a>
    <div class="p-5 transition hover:scale-110">
        <a href="#">
            <h5 class="mb-2  text-2xl text-center font-bold tracking-tight text-gray-900">Employment | रोजगार</h5>
        </a>        
    </div>
</div>

<div transition:fade class="hover:shadow-lg mx-auto max-w-sm bg-white rounded-lg border border-gray-200 shadow-md transition-all duration-200 cursor-pointer filter md:saturate-50 hover:saturate-100">
    <a href="#">
        <img class="p-3 rounded-t-lg" src={serv} alt="">
    </a>
    <div class="p-5 transition hover:scale-110">
        <a href="#">
            <h5 class="mb-2  text-2xl text-center font-bold tracking-tight text-gray-900">Services | सेवाएं</h5>
        </a>        
    </div>
</div>

</div>