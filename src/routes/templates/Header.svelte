<div class="top-header"></div>

<svelte:window bind:scrollY={scrollY} on:scroll={checkIfSticky}/>

<header id="header" class:sticky={stickyClass === true}>

    <div class="left-header">
        <img src="/images/logoCFSE.png" alt="logo" class="img-header" on:click={goLanding} on:keypress={goLanding}>
    </div>

    <div class="right-header">

        <div class="list-right-header">

            <a id="activities-header" on:click={goTo('.container-activities')} on:keypress={goTo('.container-activities')}>Activités</a>
            <a id="mission-header" on:click={goTo('.container-mission')} on:keypress={goTo('.container-mission')}>Mission</a>
            <a id="values-header" on:click={goTo('.container-values')} on:keypress={goTo('.container-values')}>Valeurs</a>
            <a id="pricings-header" on:click={goTo('.container-pricing')} on:keypress={goTo('.container-pricing')}>Tarifs</a>

        </div>

        <Button textButton="Nous contacter"/>

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
                height: auto;
                transition: .4s;

                &:hover {
                    cursor: pointer;
                }
            }

        }

        .right-header {
            display: flex;
            flex-direction: row;
            align-items: center;
            gap: space(5);

            .list-right-header {
                display: flex;
                flex-direction: row;
                align-items: center;
                gap: space(5);
                font-family: $font-opensans;
                font-size: 1.15rem;
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
                    text-decoration: none;
                    transition: .4s;
                    
                    &:hover {
                        cursor: pointer;
                        background-position: 0 100%;
                    }

                }
            }
        }
    }

    @media screen and (max-width: $xl) {

        .top-header {
            padding-top: 15px;
        }
        
        #header {
            height: 70px;
            padding: 0 space(3) 0 space(3);

            .left-header {

                .img-header {
                    width: 60px;
                }
            }

            .right-header {
                gap: space(3);

                .list-right-header {
                    gap: space(2.5);
                    font-size: 1rem;
                }
            }
        }
    }

    @media screen and (max-width: $m) {



        #header {

            .right-header {

                .list-right-header {

                    display: none!important;
                }
            }
        }

    }

</style>

<script lang="ts">
    import Button from "./Button.svelte";

    let scrollY: number;
    let stickyClass: boolean = false;

    function checkIfSticky(): void {   

        if(scrollY > 30) {
            stickyClass = true;
            
        } else {
            stickyClass = false;
        }
        
    }

    function goLanding(): void {
        window.scrollTo(
            {
                top: 0,
                left: 0,
                behavior: "smooth"
            }
        );
    }

    function getHeaderHeight(): number {
        const header = document.querySelector('#header');
        const height = header!.getBoundingClientRect().height;

        return height;
    }

    const goTo = (container: string) => () => {
        const containerDOM = document.querySelector(container);
        const height = (containerDOM!.getBoundingClientRect().top + window.scrollY) - getHeaderHeight();

        window.scrollTo(
            {
                top: height,
                left: 0,
                behavior: "smooth"
            }
        );
    }

</script>

