<main class="container-landing">

    <div class="background-landing"></div>
    
    <section class="container-hero">

        <div class="container-hero-top">
            
            <div class="container-hero-top-left">
                <img src="images/hero-banner.png" alt="hero-banner" class="hero-img">
            </div>

            <div class="container-hero-top-right">

                <h2 class="hero-title">
                    Confiance & Sérénité
                </h2>

                <p class="hero-description">
                    Nous sommes là pour vous offrir le soutien dont vous avez besoin, 
                    quelles que soient vos difficultés. Que vous soyez seul, en famille ou en couple, 
                    que vous ayez des problèmes de santé, financiers ou sociaux, nous sommes là pour vous écouter et vous aider.
                    <br/><br/>
                    N'hésitez pas à nous contacter pour en savoir plus sur nos services et sur les moyens de nous soutenir. 
                    Ensemble, nous pouvons faire la différence dans la vie des personnes qui en ont le plus besoin. 
                </p>

                <div class="hero-button">
                    <Button textButton = "Nous contacter"/>
                </div>

            </div>

        </div>

        <div class="container-hero-bottom">

            <div class="container-hero-points">

                <div class="hero-point">

                    <h1 class="hero-point-title">Le soutien personnalisé</h1>

                    <p class="hero-point-text">
                        L'association offre des services adaptés aux besoins uniques de chaque personne, 
                        avec une attention particulière aux individus qui ont des besoins spécifiques liés à la santé ou au bien-être.
                    </p>

                </div>

                
                <div class="hero-point">

                    <h1 class="hero-point-title">Équipe qualifiée</h1>

                    <p class="hero-point-text">
                        L'expertise et les compétences de l'équipe de professionnels de l'association, qui ont une grande expérience dans le secteur sanitaire et social.
                    </p>

                </div>

                
                <div class="hero-point">

                    <h1 class="hero-point-title">Écoute et empathie</h1>

                    <p class="hero-point-text">
                        L'écoute et l'empathie de l'équipe de l'association envers les personnes aidées, 
                        pour leur offrir un accompagnement adapté à leur situation personnelle.
                    </p>

                </div>
            </div>
        </div>

    </section>

</main>

<style global lang="scss">

    $animation-duration: .5s;

    .container-landing {
        width: 100%;
        height: calc(100vh - 130px);
        min-height: 590px;
        position: relative;
        display: flex;
        justify-content: center;
        align-items: center;
        
        .background-landing {
            position: absolute;
            width: 100%;
            height: calc(100vh - 130px);
            min-height: 590px;
            top: -65px;
            left: 0;
            z-index: -100;
            background: url(/images/backgroundWave.svg) no-repeat center center fixed; 
            -webkit-background-size: cover;
            -moz-background-size: cover;
            -o-background-size: cover;
            background-size: cover;
            background-attachment: scroll;
        }

        .container-hero {
            position: relative;
            width: 100%;
            height: calc(100vh - 130px);
            min-height: 590px;
            display: flex;
            flex-direction: column;

            .container-hero-top {
                display: flex;
                flex-direction: row;
                flex: 6;
                transition: .4s ease;

                .container-hero-top-left {
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    flex: 7;

                    .hero-img {
                        width: 35%;
                        height: auto;
                        animation: slideInLeft $animation-duration ease-in-out both;
                    }
                }

                .container-hero-top-right {
                    display: flex;
                    flex-direction: column;
                    flex: 5;
                    justify-content: space-around;
                    height: 100%;
                    padding: space(4) 0 space(4) 0;
                    gap: space(2);
                    animation: slideInRight $animation-duration ease-in-out both;
                    animation-delay: calc(.5s - 300ms);                    

                    .hero-title {
                        font-family: $font_opensans;
                        font-size: 3.4em;
                        font-weight: 800;
                        color: $background; 
                    }

                    .hero-description {
                        font-family: $font_opensans;
                        font-size: 1em;
                        font-weight: 400;
                        width: 70%;
                        color: $background;
                        line-height: 16pt; 
                    }

                    .hero-button {
                        width: auto;
                    }
                }
            }

            .container-hero-bottom {
                display: flex;
                flex: 4;

                .container-hero-points {
                    height: 100%;
                    width: 100%;
                    display: flex;
                    flex-direction: row;
                    justify-content: space-around;
                    align-items: center;

                    .hero-point {
                        height: 100%;
                        display: flex;
                        flex-direction: column;
                        justify-content: center;
                        align-items: center;
                        gap: space(4);
                        animation: backInUp $animation-duration ease-in-out both;

                        &:nth-child(1) {
                            animation-delay: 1s - 300ms; 
                        }

                        &:nth-child(2) {
                            animation-delay: 1.5s - 300ms; 
                        }

                        &:nth-child(3) {
                            animation-delay: 2s - 300ms; 
                        }

                        .hero-point-title {
                            font-family: $font_montserrat;
                            font-size: 1.6em;
                            font-weight: bold;
                            color: $text;
                        }

                        .hero-point-text {
                            width: 80%;
                            font-family: $font_montserrat;
                            font-size: 1em;
                            font-weight: bold;
                            text-align: center;
                            color: $text;
                        }
                    }
                }
            }
        }

    }

    @keyframes fadeInDown {
        from {
            opacity: 0;
            transform: translate3d(0, -100%, 0);
        }

        to {
            opacity: 1;
            transform: translate3d(0, 0, 0);
        }
    }

    @keyframes slideInLeft {
        from {
            transform: translate3d(-150%, 0, 0);
            visibility: visible;
        }

        to {
            transform: translate3d(0, 0, 0);
        }
    }

    @keyframes slideInRight {
        from {
            transform: translate3d(150%, 0, 0);
            visibility: visible;
        }

        to {
            transform: translate3d(0, 0, 0);
        }
    }

    @keyframes backInUp {
        0% {
            transform: translateY(1200px) scale(0.7);
            opacity: 0;
        }

        80% {
            transform: translateY(0px) scale(0.7);
            opacity: 0.7;
        }

        100% {
            transform: scale(1);
            opacity: 1;
        }
    }

    @media screen and (max-width: 1500px) {

        .container-landing {

            .container-hero {

                .container-hero-top {

                    .container-hero-top-left {
                        flex: 1.5;

                        .hero-img {
                            width: 45%;
                        }
                    }

                    .container-hero-top-right {
                        flex: 2;

                        .hero-title {
                            font-size: 2.8em;
                        }

                        .hero-description {
                            font-size: 1em;
                            width: 80%;
                        }
                    }
                }

                .container-hero-bottom {

                    .container-hero-points {

                        .hero-point {

                            .hero-point-text {
                                width: 75%;
                            }
                        }
                    }
                }
            }
        }
    }

    @media screen and (max-width: $xxl) {

        .container-landing {

            .background-landing {
                top: -50px;
            }

            .container-hero {

                .container-hero-top {
                    justify-content: center;
                    align-items: center;
                    gap: space(4);

                    .container-hero-top-left {
                        flex: 1.5;

                        .hero-img {
                            width: 55%;
                        }
                    }

                    .container-hero-top-right {
                        flex: 2;
                        justify-content: space-evenly;

                        .hero-title {
                            font-size: 2.2em;
                        }

                        .hero-description {
                            font-size: 0.9em;
                            width: 90%;
                        }
                    }
                }

                .container-hero-bottom {
                    
                    .container-hero-points {

                        .hero-point {

                            .hero-point-title {
                                font-size: 1.4em;
                            }

                            .hero-point-text {
                                font-size: 0.9em;
                            }
                        }
                    }
                }
            }
        }
    }

    @media screen and (max-width: $xl) {

        .container-landing {
            height: calc(100vh - 85px);

            .background-landing {
                height: calc(100vh - 85px);
                top: -42px;
            }

            .container-hero {
                height: calc(100vh - 85px);

                .container-hero-top {

                    .container-hero-top-left {

                        .hero-img {
                            width: 60%;
                        }
                    }

                    .container-hero-top-right {

                        .hero-title {
                            font-size: 1.8em;
                        }

                    }
                }

                .container-hero-bottom {
                    
                    .container-hero-points {

                        .hero-point {

                            .hero-point-title {
                                font-size: 1.2em;
                            }

                            .hero-point-text {
                                font-size: 0.9em;
                            }
                        }
                    }
                }
            }
        }
    }

    @media screen and (max-width: $l) {

        .container-landing {

            .container-hero {
                gap: 6vh;

                .container-hero-top {
                    padding-left: space(4);
                    padding-right: space(4);
                    padding-top: 3vh;

                    .container-hero-top-left {
                        display: none;

                        .hero-img {
                            width: 80%;
                        }
                    }

                    .container-hero-top-right {
                        flex: none;
                        width: 100%;

                        .hero-description {
                            width: 100%;
                        }
                        
                    }
                }

                .container-hero-bottom {
                    padding-bottom: 3vh;
                    
                    .container-hero-points {
                        flex-direction: column;
                        justify-content: center;

                        .hero-point {
                            gap: space(1);

                            .hero-point-title {
                                font-size: 1.1em;
                            }

                            .hero-point-text {
                                font-size: 0.8em;
                            }
                        }
                    }
                }
            }
        }
    }

    @media screen and (max-width: $m) {

        .container-landing {
            height: calc(110vh - 85px);

            .background-landing {
                height: calc(110vh - 85px);
            }
            
            .container-hero {
                height: calc(110vh - 85px);

                .container-hero-top {
                    padding-top: 0vh;

                    .container-hero-top-right {
                        padding: 0;

                        .hero-description {
                            font-size: 0.85em;
                        }
                        
                    }
                }

                .container-hero-bottom {
                    
                    .container-hero-points {

                        .hero-point {

                            .hero-point-title {
                                font-size: 1em;
                            }

                            .hero-point-text {
                                font-size: 0.75em;
                            }
                        }
                    }
                }
            }
        }
    }

    @media screen and (max-width: $s) {

        .container-landing {
            height: calc(150vh - 85px);

            .background-landing {
                height: calc(150vh - 85px);
            }
            
            .container-hero {
                height: calc(150vh - 85px);
            }
        }
    }   


</style>

<script lang=ts>

    import Button from '../templates/Button.svelte';
    import { Parallax, ParallaxLayer } from 'svelte-parallax'


</script>
