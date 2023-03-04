<section class="container-pricing">

    <h3 class="pricing-title">
        <span id="title_firstline">Les tarifs de<br></span>
        <span id="title_secondline">Confiance & Sérénité</span>
    </h3>

    <div class="pricing-hero">

        <div class="pricing-hero-top" use:reveal={{ transition : "fly", duration : 300 }}>

            <img src="/images/pricing.png" alt="pricing" class="pricing-img">

        </div>

        <div class="pricing-hero-bottom" use:reveal={{ transition : "blur", duration : 300 }}>

            <div class="pricing-text">
    
                <div class="pricing-text-wrapper">
                    <p class="pricing-text-title">
                        Majoration des tarifs : 
                    </p>
                    <p>
                        Entre 22h et 6h : majoration de 25%
                    </p>
                    <p>
                        1er Mai et 25 Décembre : majoration de 100%
                    </p>
                    <p>
                        Indémnités kilométriques
                    </p>
                </div>
    
            </div>

        </div>

    </div>

</section>

<section class="container-pricing-advantages">

    <h3 class="pricing-advantages-title">
        <span>Avantages fiscaux</span>
    </h3>

    <div class="pricing-advantages-text">

        <div class="pricing-advantages-text-wrapper">
            <p use:reveal={{ transition : "blur", duration : 500, delay: 200}}>
                Il existe différentes aides fiscales pour les personnes bénéficiant de services d’aides à domicile :
            </p><br>
            <p use:reveal={{ transition : "blur", duration : 500, delay: 200}}>
                Le crédit d’impôt permet de bénéficier d’un remboursement lorsque le montant du crédit d’impôt est
                supérieur à l’impôt à payer, les personnes non imposables peuvent en bénéficier.
            </p><br>
            <p use:reveal={{ transition : "blur", duration : 500, delay: 200}}>
                La réduction d’impôt permet uniquement de diminuer voir d’annuler l’impôt, par conséquent les personnes
                non imposables ne peuvent pas en bénéficier.
            </p><br>
            <p use:reveal={{ transition : "blur", duration : 500, delay: 200}}>
                Dans le cadre des prestations de services proposées par CONFIANCE & SERENITE vous pouvez bénéficier d’un
                crédit d’impôt égal à 50% des dépenses annuelles engagées.
            </p><br>
            <p use:reveal={{ transition : "blur", duration : 500, delay: 200}}>
                Exemple : vous payez 6000€ d’aide à domicile en 2022. Vous pourrez bénéficier d’un crédit d’impôt de 3000€ (50%
                de 6000€) sur vos impôts en 2023.
            </p><br>
            <p use:reveal={{ transition : "blur", duration : 500, delay: 200}}>
                Pour rappel les prestations vous donnant droit à un crédit d’impôt sont :
            </p><br>
            <p use:reveal={{ transition : "blur", duration : 500, delay: 200}}>
                - L’aide dans les acte de la vie quotidienne.
            </p><br>
            <p use:reveal={{ transition : "blur", duration : 500, delay: 200}}>
                - L’entretien de la maison et les travaux ménagers.
            </p><br>
            <p use:reveal={{ transition : "blur", duration : 500, delay: 200}}>
                Les montants sont plafonnés (12 000€ majoré de 1 500€ par personne de + de 65 ans au sein du foyer et
                plafonnée à 20 000€ si la personne titulaire de la carte d’invalidité ou mobilité inclusion invalidité ou si la
                personne perçoit une pension d’invalidité de cat 3).
            </p><br>
            <p use:reveal={{ transition : "blur", duration : 500, delay: 200}}>
                Vous bénéficier de l’APA ou de la PCH dans ce cas le crédit d’impôt s’appliquera sur le montant égal à la
                différence entre le montant de la facture et le montant de l’aide perçue.
            </p><br>
            <p use:reveal={{ transition : "blur", duration : 500, delay: 200}}>
                <a href="https://www.impots.gouv.fr/particulier/emploi-domicile" target="_blank" rel="noreferrer">https://www.impots.gouv.fr/particulier/emploi-domicile</a> 
            </p>
        </div>

    </div>

</section>

<style global lang="scss">

    .container-pricing {
        width: 100%;
        min-height: calc(100vh - 100px);
        height: auto;
        display: flex;
        flex-direction: column;

        .pricing-title {

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

        .pricing-hero {
            display: flex;
            flex-direction: column;
            align-self: center;
            justify-content: space-around;
            width: 70%;
            height: 100%;
            padding: space(6) 0 space(6) 0;
            gap: space(4);

            .pricing-hero-top {
                display: flex;

                .pricing-img {
                    width: 100%;
                    height: auto;
                }

            }

            .pricing-hero-bottom {

                .pricing-text {
                    font-family: $font_montserrat;
                    font-weight: 400;
                    font-size: 1em;
                    color: $text;
                    line-height: 16pt;

                    .pricing-text-title {
                        font-weight: 700;
                    }
                }
            }

        }

    }

    .container-pricing-advantages {
        width: 100%;
        height: auto;
        display: flex;
        flex-direction: column;

        .pricing-advantages-title {
            font-family: $font_opensans;
            font-size: 2.8em;
            color: $text;
            font-weight: 600;
            padding-left: 4vw;
        }

        .pricing-advantages-text {
            display: flex;
            height: 100%;
            width: 80vw;
            line-height: 16pt;
            padding: 48px 0 48px 4vw;

            .pricing-advantages-text-wrapper {
                align-self: center;
                font-family: $font_montserrat;
                font-weight: 400;
                font-size: 1.1em;
                color: $text;
            }
        }
    }

    @media screen and (max-width: 1500px) {

        .container-pricing {

            min-height: auto;
            padding-top: 100px;

            .pricing-title {
                font-size: 2.4em;
            }

        }

        .container-pricing-advantages {

            .pricing-advantages-title {
                font-size: 2.4em;
            }

            .pricing-advantages-text {
                width: 90vw;
            }
        }
    }

    @media screen and (max-width: $xxl) {

        .container-pricing {

            .pricing-title {

                font-size: 2.2em;

            }

            .pricing-hero {
                width: 80%;
            }

        }

        .container-pricing-advantages {

            .pricing-advantages-title {
                font-size: 2.2em;
            }

            .pricing-advantages-text {

                .pricing-advantages-text-wrapper {
                    font-size: 1em;
                }
            }
        }
    }

    @media screen and (max-width: $l) {

        .container-pricing {

            padding-top: 70px;

            .pricing-title {

                font-size: 2em;

            }

            .pricing-hero {
                width: 90%;

                .pricing-hero-bottom {

                    .pricing-text {
                        font-size: 0.9em;
                    }
                }
            }
        }

        .container-pricing-advantages {

            .pricing-advantages-title {
                font-size: 2em;
            }

            .pricing-advantages-text {
                
                .pricing-advantages-text-wrapper {
                    font-size: 0.9em;
                }
            }
        }
    }

    @media screen and (max-width: $m) {

        .container-pricing {

            .pricing-title {

                font-size: 1.8em;

            }

        }

        .container-pricing-advantages {

            .pricing-advantages-title {
                font-size: 1.8em;
            }

            .pricing-advantages-text {

                .pricing-advantages-text-wrapper {
                    font-size: 0.9em;
                }

            }
        }
    }
</style>

<script lang="ts">
    import { reveal } from 'svelte-reveal';
</script>