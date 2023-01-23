<div class="top-header"></div>

<svelte:window bind:scrollY={scrollY} on:scroll={checkIfSticky}/>

<header id="header" class:sticky={stickyClass === true}>

    <div class="left-header">
        <img src="/images/logoCFSE.png" alt="logo" class="img-header">
    </div>

    <div class="right-header">

        <div class="list-right-header">

            <a id="activities-header">Activités</a>
            <a id="mission-header">Mission</a>
            <a id="values-header">Valeurs</a>
            <a id="pricings-header">Tarifs</a>

        </div>

        <Button textButton="Nous contacter" />

    </div>


</header>

<style global lang="scss">

    .top-header {
        background-color: $primary;
        padding-top: 30px;
    }

    .sticky {
        position: sticky;
        position: -webkit-sticky;
        position: -moz-sticky;
        position: -ms-sticky;
        position: -o-sticky;
        top: 0;
        width: 100%;
    }

    #header {
        background-color: $primary;
        width: 100%;
        height: 100px;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
        z-index: 1;
        padding: 0 space(6) 0 space(6);

        .left-header {

            .img-header {
                width: 75px;
                height: 61px;

                &:hover {
                    cursor: pointer;
                }
            }

        }

        .right-header {
            display: flex;
            flex-direction: row;
            align-items: center;
            gap: space(6);

            .list-right-header {
                display: flex;
                flex-direction: row;
                align-items: center;
                gap: space(5);
                font-family: $font-opensans;
                font-size: 1.15em;
                font-weight: bold;
                color: $background;

                a {

                    position: relative;
                    display: inline-block;
                    overflow: hidden;
                    background: linear-gradient(to right, $text, $text 50%, $background 50%);
                    background-clip: text;
                    -webkit-background-clip: text;
                    -webkit-text-fill-color: transparent;
                    background-size: 200% 100%;
                    background-position: 100%;
                    transition: background-position 275ms ease;
                    text-decoration: none; // text decorations are clipped in WebKit browsers
                    
                    &:hover {
                        cursor: pointer;
                        background-position: 0 100%;
                    }

                }
            }
        }
    }

</style>

<script lang="ts">
    import Button from "./Button.svelte";

    let scrollY: number;
    let stickyClass: boolean = false;

    function checkIfSticky() {   

        if(scrollY > 30) {
            stickyClass = true;
            
        } else {
            stickyClass = false;
        }
        
    }

</script>

