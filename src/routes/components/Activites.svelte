<section class="container-activities">

    <h3 class="activities-title">
        <span id="title_firstline">Les activités de<br></span>
        <span id="title_secondline">Confiance & Sérénité</span>
    </h3>

    <div class="activities-list">

        <div class="activities-card">

            <img src="images/activities-washing.png" alt="activité" class="activities-img">

            <h2 class="activities-text">Entretien de la maison et travaux ménagers</h2>

        </div>

        <div class="activities-card">

            <img src="images/activities-nursing.png" alt="activité" class="activities-img">

            <h2 class="activities-text">Assistance aux personnes agées / handicapées</h2>

        </div>

        <div class="activities-card">

            <img src="images/activities-gardening.png" alt="activité" class="activities-img">

            <h2 class="activities-text">Jardinage et entretien des espaces verts et bricolage</h2>

        </div>

    </div>

</section>

<style global lang="scss">

    .container-activities {
        width: 100%;
        height: 100vh;
        min-height: 100vh;
        position: relative;
        display: flex;
        flex-direction: column;
        padding-top: 100px;

        .activities-title {

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

        .activities-list {
            display: flex;
            flex-direction: row;
            align-items: center;
            width: 100%;
            height: 100%;

            .activities-card {
                display: flex;
                flex-direction: column;
                align-items: center;
                flex: 1;
                padding-left: space(6);
                padding-right: space(6);

                .activities-img {
                    width: 400px;
                    height: 400px;
                }
                .activities-text {
                    font-family: $font_montserrat;
                    font-weight: bold;
                    font-size: 1.5em;
                    color: $text;
                    text-align: center;
                }
            }
        }

    }
</style>