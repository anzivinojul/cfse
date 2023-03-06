<section class="container-activities">

    <h3 class="activities-title">
        <span id="title_firstline">Les activités de<br></span>
        <span id="title_secondline">Confiance & Sérénité</span>
    </h3>

    <div class="activities-list">

        <div class="activities-card" use:reveal={{ transition : "fly", duration : 500 }}>

            <img src="images/activities-washing.png" alt="activité" class="activities-img">

            <h2 class="activities-text">Entretien de la maison et travaux ménagers</h2>

        </div>

        <div class="activities-card" use:reveal={{ transition : "fly", duration : 500, delay: 300 }}>

            <img src="images/activities-nursing.png" alt="activité" class="activities-img">

            <h2 class="activities-text">Assistance aux personnes agées / handicapées</h2>

        </div>

        <div class="activities-card" use:reveal={{ transition : "fly", duration : 500, delay: 600 }}>

            <img src="images/activities-gardening.png" alt="activité" class="activities-img">

            <h2 class="activities-text">Jardinage et entretien des espaces verts et bricolage</h2>

        </div>

    </div>

</section>

<style global lang="scss">

    .container-activities {
        width: 100%;
        height: calc(100vh - 100px);
        min-height: 590px;
        position: relative;
        display: flex;
        flex-direction: column;

        .activities-title {

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
                    width: 80%;
                    height: 80%;
                }

                .activities-text {
                    font-family: $font_montserrat;
                    font-weight: bold;
                    font-size: clamp(0.9rem, 1.8vw, 1.5rem);
                    color: $text;
                    text-align: center;
                }
            }
        }

    }

    @media screen and (max-width: $xxl) {

        .container-activities {

            height: auto;
            padding-top: 100px;

            .activities-list {
                flex-direction: column;
                align-items: center;
                width: 100%;
                height: 100%;

                .activities-card {
                    display: flex;
                    flex-direction: row;
                    align-items: center;
                    flex: 1;

                    .activities-img {
                        width: 40%;
                        min-width: 250px;
                        height: auto;
                    }

                    .activities-text {
                        justify-self: center;
                        padding: 0 space(4) 0 space(4);
                        width: 80%;
                        text-align: start;
                    }
                }
            }
        }
    }

    @media screen and (max-width: $l) {

        .container-activities {

            padding-top: 70px;

            .activities-list {

                .activities-card {
                    padding-left: space(2);
                    padding-right: space(2);

                    .activities-img {
                        min-width: 250px;
                    }

                    .activities-text {
                        padding: 0 space(2) 0 space(2);
                    }
                }
            }
        }
    }

    @media screen and (max-width: $m) {

        .container-activities {

            .activities-list {

                .activities-card {
                    padding-left: 0;
                    padding-right: 0;

                    .activities-img {
                        min-width: 200px;
                    }

                    .activities-text {
                        padding: 0 space(1) 0 space(1);
                    }
                }
            }
        }
    }

</style>

<script lang="ts">
    import { reveal } from 'svelte-reveal';
</script>