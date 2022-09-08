<script>
import {isoverlayopen} from "../stores/overlay"
import Footer from "../components/footer.svelte";
import Nav from "../components/nav.svelte";
</script>

<div class="">
    <Nav/>
    <slot/>
    <Footer/>
</div>


<style>
@tailwind base;
@tailwind components;
@tailwind utilities;
</style>