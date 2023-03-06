<section class="container-mission">

    <h3 class="mission-title">
        <span id="title_firstline">La mission de<br></span>
        <span id="title_secondline">Confiance & Sérénité</span>
    </h3>

    <div class="mission-hero">

        <div class="mission-hero-left" id="mission-hero-left" use:reveal={{ transition : "fly", duration : 500, threshold : 0.1 }}>

            <img src="images/mission.svg" alt="mission" class="mission-img">

        </div>

        <div class="mission-hero-right">

            <div class="mission-text">

                <div class="mission-text-wrapper">
                    <p use:reveal={{ transition : "blur", duration : 500 }}>
                        L’association est née d’une volonté commune d’évoluer professionnellement vers des activités 
                        en accord avec nos valeurs que sont notamment le sens du service et la solidarité.
                    </p><br>
                    <p use:reveal={{ transition : "blur", duration : 500 }}>
                        Nous avons à cœur de travailler pour le bien-être de toute personne qu’elles soient vulnérables, 
                        dépendantes ou en situation de handicap. Notre mission étant de répondre au mieux à leur besoins actuels et à venir.
                    </p><br>
                    <p use:reveal={{ transition : "blur", duration : 500 }}>
                        Nos collaborateurs sont soigneusement recrutés et nous attachons une attention particulière à leur compétence professionnelles, 
                        leur expérience tout autant qu’à leur qualités humaines telle que l’écoute et la bienveillance.
                        En phase de recrutement, nous vérifions leurs références, nous veillons à ce que chacun participe au respect de la vie privée de nos bénéficiaires
                            en faisant preuve de réserve et de discrétion.
                    </p><br>
                    <p use:reveal={{ transition : "blur", duration : 500 }}>
                        Des réunions ou entretiens réguliers nous permettent d’évaluer en continu les besoins des bénéficiaires et de procéder à des ajustements.
                        Notre coordinatrice Amel forte d’une expérience d’une vingtaine d’années dans le secteur sanitaire et 
                        social se rendra au domicile des bénéficiaires pour évaluer avec eux leurs besoins. Elle assurera la coordination 
                        entre l’équipe d’aide à domicile et les bénéficiaires et leurs proches.
                    </p>
                </div>
    
            </div>

        </div>

    </div>

</section>

<style global lang="scss">

    .container-mission {
        width: 100%;
        height: calc(100vh - 100px);
        min-height: 590px;
        position: relative;
        display: flex;
        flex-direction: column;

        .mission-title {

            font-family: $font_opensans;
            font-size: clamp(1.6rem, 3.8vw, 2.8rem);
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

        .mission-hero {
            display: flex;
            flex-direction: row;
            width: 100%;
            height: 100%;

            .mission-hero-left {
                display: flex;
                justify-content: center;
                align-items: center;
                flex: 1;

                .mission-img {
                    width: 80%;
                    height: auto;
                    min-width: 400px;
                }
            }

            .mission-hero-right {
                display: flex;
                justify-content: center;
                align-items: center;
                flex: 2;
                padding: space(10);

                .mission-text {
                    display: flex;
                    align-self: center;
                    height: 100%;
                    line-height: 16pt; 

                    .mission-text-wrapper {
                        align-self: center;
                        font-family: $font_montserrat;
                        font-weight: 400;
                        font-size: clamp(0.9rem, 1.5vw, 1.1rem);
                        color: $text;
                        height: 80%;
                    }
                }
            }
        }
    }


    @media screen and (max-width: 1500px) {

        .container-mission {

            .mission-hero {

                .mission-hero-right {
                    padding: space(10) 0 space(10) 0;

                    .mission-text {
                        width: 90%;
                        height: auto;

                        .mission-text-wrapper {
                            height: auto;
                        }
                    }
                }
            }

        }
    }

    @media screen and (max-width: $xxl) {

        .container-mission {

            height: auto;
            padding-top: 100px;

            .mission-hero {

                .mission-hero-left {

                    .mission-img {
                        width: 100%;
                        min-width: 250px;
                    }
                }

                .mission-hero-right {
                    padding: space(10) 0 space(10) 0;
                }
            }

        }
    }

    @media screen and (max-width: $l) {

        .container-mission {

            padding-top: 70px;

            .mission-hero {
                flex-direction: column;

                .mission-hero-left {

                    .mission-img {
                        width: 40%;
                        min-width: 250px;
                    }
                }

                .mission-hero-right {
                    padding: 0 0 space(10) 0;
                }
            }
        }
    }

    @media screen and (max-width: $m) {

        .container-activities {

            .mission-hero {

                .mission-hero-left {

                    .mission-img {
                        min-width: 200px;
                    }
                }
            }
        }
    }

</style>

<script lang="ts">
    import { reveal } from 'svelte-reveal';
</script>