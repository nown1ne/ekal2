<script>
import Grid from "../components/grid.svelte";
import banner from '$lib/assets/bigbanner.png';
import { fade, blur, fly, slide, scale } from "svelte/transition";
import { quintOut } from "svelte/easing";
import Animate from "../animate.svelte";
</script>
<Animate>
     <img src="{banner}" alt="Big banner with kids" class="w-screen mb-6 brightness-75 transform hover:brightness-100 duration-500">
     <Grid/>
 </Animate> 
