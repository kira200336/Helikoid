<script>
    import {onMount} from "svelte";
    import LoadingScreen from "$lib/components/LoadingScreen.svelte";
    import Navbar from "$lib/components/navbar/Navbar.svelte";
    import Footer from "$lib/components/Footer.svelte";

    //Global scss
    import '$lib/theme/global.scss'

    let ready

    onMount(() => {
        ready = true
    });

    //If we're mounted we wait x (1 second) amount of time to make sure fonts etc is ready. Looks good as well.
    $: {
        if (ready) {
            setInterval(() => {
                state.set({loading: false})
            }, 1000)
        }
    }
</script>

<!--Layout with navbar and footer, slot is all the content being rendered in <main>, dont add a main tag elsewhere. -->
<Navbar/>
<main>
    <slot/>
</main> 
<Footer/>

