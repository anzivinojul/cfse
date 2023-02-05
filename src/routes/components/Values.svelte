<section class="container-values">

    <h3 class="values-title">
        <span id="title_firstline">Les valeurs de<br></span>
        <span id="title_secondline">Confiance & Sérénité</span>
    </h3>

    <div class="values-hero">

        <div class="values-list">

            <div class="values-card">

                <img src="images/listening.svg" alt="listening" class="values-img">
                <h3 class="values-text">Écoute</h3>
    
            </div>
    
            <div class="values-card">
    
                <img src="images/excellence.svg" alt="excellence" class="values-img">
                <h3 class="values-text">Excellence</h3>
    
            </div>

        </div>
        <div class="values-list">
    
            <div class="values-card">
    
                <img src="images/skillful.svg" alt="skillful" class="values-img">
                <h3 class="values-text">Compétents</h3>
    
            </div>
    
            <div class="values-card">
    
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
            font-size: 2.8em;
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
                    flex-direction: column;
                    align-items: center;
                    gap: space(1);

                    .values-img {
                        height: auto;
                        width: 100%;
                        min-width: 250px;
                    }

                    .values-text {
                        font-family: $font_montserrat;
                        font-weight: bold;
                        font-size: 1.8em;
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

            .values-title {
                font-size: 2.4em;
            }

            .values-hero {

                .values-list {

                    .values-card {
                        
                        .values-img {
                            min-width: 230px;
                        }

                        .values-text {
                            font-size: 1.6em;
                        }
                    }
                }
            }
        }
    }

    @media screen and (max-width: $xxl) {

        .container-values {

            .values-title {

                font-size: 2.2em;

            }

            .values-hero {

                .values-list {

                    .values-card {

                        .values-text {
                            font-size: 1.4em;
                        }
                    }
                }
            }
        }
    }

    @media screen and (max-width: $l) {

        .container-values {

            padding-top: 70px;


            .values-title {

                font-size: 2em;

            }

            .values-hero {

                .values-list {
                    gap: 0px;

                    .values-card {

                        .values-img {
                            min-width: 40vw;
                        }

                        .values-text {
                            font-size: 1.2em;
                        }
                    }
                }
            }

        }
    }

    @media screen and (max-width: $m) {

        .container-activities {

            .values-title {

                font-size: 1.8em;

            }

            .values-hero {

                .values-list {

                    .values-card {

                        .values-text {
                            font-size: 1.1em;
                        }
                    }
                }
            }

        }
    }

    @media screen and (max-width: $s) {

        .container-activities {

            .values-title {

                font-size: 1.8em;

            }

            .values-hero {

                .values-list {

                    .values-card {

                        .values-text {
                            font-size: 1.1em;
                        }
                    }
                }
            }

        }
    }
    
</style>