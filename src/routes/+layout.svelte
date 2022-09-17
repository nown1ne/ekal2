<script>
  import Animate from "../animate.svelte";
import Footer from "../components/footer.svelte";
import Nav from "../components/nav.svelte";
</script>

<div class="">
    <Animate>
        <Nav/>
        <slot/>
        <Footer/>
    </Animate>
</div>


<style>
@tailwind base;
@tailwind components;
@tailwind utilities;
</style>