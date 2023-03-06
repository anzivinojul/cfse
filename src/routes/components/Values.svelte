<section class="container-values">

    <h3 class="values-title">
        <span id="title_firstline">Les valeurs de<br></span>
        <span id="title_secondline">Confiance & Sérénité</span>
    </h3>

    <div class="values-hero">

        <div class="values-list">

            <div class="values-card" use:reveal={{ transition : "fly", duration : 500 }}>

                <h3 class="values-text">Écoute</h3>
                <img src="images/listening.svg" alt="listening" class="values-img">
    
            </div>
    
            <div class="values-card" use:reveal={{ transition : "fly", duration : 500, delay: 300 }}>
    
                <img src="images/excellence.svg" alt="excellence" class="values-img">
                <h3 class="values-text">Excellence</h3>
    
            </div>

        </div>
        <div class="values-list">
    
            <div class="values-card" use:reveal={{ transition : "fly", duration : 500 }}>
    
                <h3 class="values-text">Compétents</h3>
                <img src="images/skillful.svg" alt="skillful" class="values-img">
    
            </div>
    
            <div class="values-card" use:reveal={{ transition : "fly", duration : 500, delay: 300 }}>
    
                <img src="images/reactivity.svg" alt="reactivity" class="values-img">
                <h3 class="values-text">Réactivité</h3>
    
            </div>

        </div>

    </div>

</section>

<style global lang="scss">

    .container-values {
        width: 100%;
        min-height: calc(100vh - 100px);
        height: auto;
        position: relative;
        display: flex;
        flex-direction: column;

        .values-title {

            font-family: $font_opensans;
            font-size: clamp(1.8rem, 3.2vw, 2.8rem);
            color: $text;
            padding-top: 2vh;
            padding-left: 4vw;

            #title_firstline {
                font-weight: 500;
            }

            #title_secondline {
                font-weight: 800;
            }

        }

        .values-hero {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            justify-self: center;
            width: 100%;
            height: 100%;
            padding: space(8) 0 space(8) 0;

            .values-list {
                display: flex;
                flex-direction: row;
                justify-content: center;
                gap: 6vw;

                .values-card {
                    display: flex;
                    flex-direction: row;
                    align-items: center;
                    justify-content: space-around;
                    gap: space(2);
                    width: 30vw;

                    .values-img {
                        height: auto;
                        width: 50%;
                        min-width: 250px;
                    }

                    .values-text {
                        font-family: $font_montserrat;
                        font-weight: bold;
                        font-size: clamp(1.1rem, 2.4vw, 1.8rem);
                        color: $text;
                    }
                }
            }

            
        }

    }

    @media screen and (max-width: 1500px) {

        .container-values {

            min-height: auto;
            padding-top: 100px;

            .values-hero {

                .values-list {

                    .values-card {
                        
                        .values-img {
                            min-width: 230px;
                        }
                    }
                }
            }
        }
    }

    @media screen and (max-width: $xxl) {

        .container-values {

            .values-hero {

                .values-list {

                    flex-direction: column;
                    gap: 0px;

                    .values-card {
                        width: 50vw;

                        &:nth-child(2n+1) {
                            flex-direction: row-reverse;
                        }

                        .values-img {
                            width: 30%;
                            min-width: 200px;
                        }

                        .values-text {
                            padding-right: space(5);
                        }
                    }
                }
            }
        }
    }

    @media screen and (max-width: $l) {

        .container-values {

            padding-top: 70px;

            .values-hero {

                .values-list {

                    .values-card {
                        width: 70vw;
                    }
                }
            }

        }
    }

    @media screen and (max-width: $m) {

        .container-values {

            .values-hero {

                .values-list {

                    .values-card {
                        width: 90vw;

                        .values-img {
                            min-width: 180px;
                            width: 180px;
                        }
                    }
                }
            }

        }
    }
    
</style>

<script lang="ts">
    import { reveal } from 'svelte-reveal';
</script>