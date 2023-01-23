<section class="container-mission">

    <h3 class="mission-title">
        <span id="title_firstline">La mission de<br></span>
        <span id="title_secondline">Confiance & Sérénité</span>
    </h3>

    <div class="mission-hero">

        <img src="images/mission.svg" alt="mission" class="mission-img">

        <div class="mission-text">

            <div class="mission-text-wrapper">
                <p>
                    L’association est née d’une volonté commune d’évoluer professionnellement vers des activités 
                    en accord avec nos valeurs que sont notamment le sens du service et la solidarité.
                </p><br>
                <p>
                    Nous avons à cœur de travailler pour le bien-être de toute personne qu’elles soient vulnérables, 
                    dépendantes ou en situation de handicap. Notre mission étant de répondre au mieux à leur besoins actuels et à venir.
                </p><br>
                <p>
                    Nos collaborateurs sont soigneusement recrutés et nous attachons une attention particulière à leur compétence professionnelles, 
                    leur expérience tout autant qu’à leur qualités humaines telle que l’écoute et la bienveillance.
                    En phase de recrutement, nous vérifions leurs références, nous veillons à ce que chacun participe au respect de la vie privée de nos bénéficiaires
                        en faisant preuve de réserve et de discrétion.
                </p><br>
                <p>
                    Des réunions ou entretiens réguliers nous permettent d’évaluer en continu les besoins des bénéficiaires et de procéder à des ajustements.
                    Notre coordinatrice Amel forte d’une expérience d’une vingtaine d’années dans le secteur sanitaire et 
                    social se rendra au domicile des bénéficiaires pour évaluer avec eux leurs besoins. Elle assurera la coordination 
                    entre l’équipe d’aide à domicile et les bénéficiaires et leurs proches.
                </p>
            </div>

        </div>

    </div>

</section>

<style global lang="scss">

    .container-mission {
        width: 100%;
        height: 100vh;
        min-height: 100vh;
        position: relative;
        display: flex;
        flex-direction: column;
        padding-top: 100px;

        .mission-title {

            font-family: $font_opensans;
            font-size: 2.8em;
            color: $text;
            padding-top: 20px;
            padding-left: 65px;

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
            
            .mission-img {
                flex: 1;
                width: auto;
                height: 80%;
                min-height: 400px;
            }

            .mission-text {
                display: flex;
                flex: 2;
                height: 100%;
                line-height: 16pt; 

                .mission-text-wrapper {
                    padding: space(10);
                    font-family: $font_montserrat;
                    font-weight: 400;
                    font-size: 1.1em;
                    color: $text;
                    height: 80%;
                }
            }
        }

    }
</style>