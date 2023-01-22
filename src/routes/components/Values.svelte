<section class="container-values">

    <h3 class="values-title">
        <span id="title_firstline">La valeurs de<br></span>
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

<style lang="scss">

    @import '../../app.scss';

    .container-values {
        width: 100%;
        height: 100vh;
        min-height: 100vh;
        position: relative;
        display: flex;
        flex-direction: column;
        padding-top: 100px;

        .values-title {

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

        .values-hero {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            width: 100%;
            height: 100%;

            .values-list {
                display: flex;
                flex-direction: row;
                justify-content: center;
                gap: space(16);

                .values-card {
                    display: flex;
                    flex-direction: column;
                    align-items: center;
                    gap: space(2);

                    .values-img {
                        height: auto;
                        width: 250px;
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
</style>