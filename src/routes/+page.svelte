<script>
    import Activites from "./components/Activites.svelte";
    import Landing from "./components/Landing.svelte";
    import Mission from "./components/Mission.svelte";
    import Values from "./components/Values.svelte";
    import Header from "./templates/Header.svelte";
</script>

<Header />
<Landing />
<Activites />
<Mission />
<Values />

<main id="next">
    <h2>IN PROGRESS</h2>
    
</main>


<style global lang="scss">
    
    #next {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 100%;
        min-height: 100vh;
        background-color: $secondary;

        h2 {
            font-family: $font_montserrat;
            font-size: 3em;
            font-weight: 900;
            color: $text;
        }
    }

</style>
