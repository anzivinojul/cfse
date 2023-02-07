<script>
    import Activites from "./components/Activites.svelte";
    import Contact from "./components/Contact.svelte";
    import Landing from "./components/Landing.svelte";
    import Mission from "./components/Mission.svelte";
    import Pricing from "./components/Pricing.svelte";
    import Values from "./components/Values.svelte";
    import Header from "./templates/Header.svelte";
</script>

<Header />
<Landing />
<Activites />
<Mission />
<Values />
<Pricing />
<Contact />

<svelte:head>
    <title>Confiance & Sérénité</title>
    <meta name ="description" content="Confiance & Sérénité est une association d'aide à la personne.">
    <script type="application/ld+json">
    {
        "@context": "http://schema.org",
        "@type": "WebSite",
            "name": "Confiance & Sérénité",
            "description": "Confiance & Sérénité est une association d'aide à la personne.",
            "url": "https://cfse.netlify.app/"
    }
    </script>
</svelte:head>