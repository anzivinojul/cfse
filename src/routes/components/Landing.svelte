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

<style lang="scss">

    @import '../../app.scss';

    .container-landing {
        width: 100%;
        min-height: calc(100vh - 130px);
        position: relative;
        display: flex;
        justify-content: center;
        align-items: center;
        
        .background-landing {
            position: absolute;
            width: 100%;
            height: 100%;
            top: -10%;
            left: 0;
            z-index: -100;
            background: url(images/backgroundWave.svg) no-repeat center center fixed; 
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
            min-width: 750px;
            min-height: 490px;
            display: flex;
            flex-direction: column;
            gap: space(8);

            .container-hero-top {
                display: flex;
                flex-direction: row;
                flex: 6;

                .container-hero-top-left {
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    flex: 7;

                    .hero-img {
                        width: 400px;
                        height: 400px;
                    }
                }

                .container-hero-top-right {
                    display: flex;
                    flex-direction: column;
                    flex: 5;
                    justify-content: space-around;

                    .hero-title {
                        font-family: $font_opensans;
                        font-size: 3.4em;
                        font-weight: bold;
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
                    min-height: 100%;
                    width: 100%;
                    display: flex;
                    flex-direction: row;
                    justify-content: space-around;
                    align-items: center;

                    .hero-point {
                        height: 100%;
                        display: flex;
                        flex-direction: column;
                        justify-content: space-evenly;
                        align-items: center;

                        .hero-point-title {
                            font-family: $font_montserrat;
                            font-size: 1.8em;
                            font-weight: bold;
                            color: $text;
                        }

                        .hero-point-text {
                            width: 80%;
                            font-family: $font_montserrat;
                            font-size: 1.1em;
                            font-weight: bold;
                            text-align: center;
                            color: $text;
                        }
                    }
                }
            }
        }

    }
</style>

<script lang=ts>

    import Button from '../templates/Button.svelte';
    import { Parallax, ParallaxLayer } from 'svelte-parallax'


</script>
