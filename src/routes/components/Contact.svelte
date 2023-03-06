<section class="container-contact">

    <div class="contact-hero">

        <div class="contact-hero-left">

            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2900.45557991881!2d5.3573603!3d43.367497300000004!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.
            1!3m3!1m2!1s0x12c9ea85e2b957cb%3A0x7ea8d111a030dc8a!2s16%20Av.%20de%20Saint-Antoine%2C%2013015%20Marseille!5e0!3m2!1sfr!2sfr!4v1675634141875!5m2!1sfr!2sfr" 
            class="contact-map" loading="lazy" title="map-location" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>

        <div class="contact-hero-right">
            
            <h3 class="contact-title">
                Restez en contact
            </h3>

            <div class="contact-details-box">

                <div class="contact-details-left">

                    <div class="contact-details">
    
                        <div class="contact-details-title">LOCALISATION</div>
                        <div class="contact-details-content">
                            <p>16 Avenue de Saint-Antoine</p>
                            <p>13015 Marseille</p>
                        </div>
        
                    </div>
        
                    <div class="contact-details">
        
                        <div class="contact-details-title">CONTACTEZ-NOUS</div>
                        <div class="contact-details-content">
                            <p>Téléphone : 04 91 60 19 96</p>
                            <p>E-mail : confiance-serenite@hotmail.com</p>
                        </div>
        
                    </div>
        
                    <div class="contact-details">
        
                        <div class="contact-details-title">NOS HORAIRES</div>
                        <div class="contact-details-content">
                            <p>LUN-VEN 09:00 - 12:00 / 13:00 - 17:00</p>
                        </div>
        
                    </div>
    
                </div>

                <div class="contact-details-right">
                    <div class="contact-image">
                        <img src="images/contact.svg" alt="contact" class="contact-img">
                    </div>
                </div>

            </div>

        </div>

    </div>

</section>

<style global lang="scss">

    .container-contact {
        width: 100%;
        height: auto;
        border-top: 2px solid $text;
        background-color: $primary;

        .contact-hero {
            display: flex;
            flex-direction: row;
            width: 100%;
            height: auto;
            padding: 120px 0 120px 0;

            .contact-hero-left {
                display: flex;
                justify-content: center;
                align-items: center;
                height: auto;
                flex: 1;

                .contact-map {
                    width: 600px;
                    height: 450px;
                    border: 2px solid $text;
                }
            }

            .contact-hero-right {
                display: flex;
                flex-direction: column;
                align-self: center;
                height: 350px;
                width: auto;
                flex: 1;

                .contact-title {
                    font-family: $font_opensans;
                    font-size: 2.8em;
                    color: $text;
                    font-weight: 600;
                }

                .contact-details-box {
                    display: flex;
                    flex-direction: row;
                    justify-content: space-between;
                    width: 100%;
                    height: 100%;

                    .contact-details-left {
                        display: flex;
                        flex-direction: column;
                        justify-content: space-around;
                        height: 100%;
                        flex: 1;

                        .contact-details {
                            display: flex;
                            flex-direction: column;
                            gap: space(2);
                            font-family: $font_opensans;
                            font-size: 1em;
                            color: $text;
                            font-weight: 500;
                        }

                    }

                    .contact-details-right {
                        display: flex;
                        flex: 1;

                        .contact-image {
                            display: flex;
                            justify-content: center;
                            width: 100%;
                            height: 100%;

                            .contact-img {
                                height: 100%;
                                width: auto;
                            }
                        }
                    }
                }
            }
        }
    }

    @media screen and (max-width: 1500px) {

        .container-contact {

            .contact-hero {

                .contact-hero-left {

                    .contact-map {
                        width: 500px;
                        height: 375px;
                    }

                }

                .contact-hero-right {
                    height: 350px;
                    
                    .contact-title {
                        padding-left: 4vw;
                        font-size: 2.6em;
                    }

                    .contact-details-box {
                        padding-left: 4vw;

                        .contact-details-left {
                            
                            .contact-details {
                                font-size: 0.95em;
                            }

                        }

                        .contact-details-right {
                            display: none;
                        }
                    }
                }
            }
        }
    }

    @media screen and (max-width: $xxl) {

        .container-contact {

            .contact-hero {
                flex-direction: column;
                gap: space(5);

                .contact-hero-right {
                    height: 300px;
                    flex: none;

                    .contact-details-box {
                        padding-left: 0px;
                        justify-content: center;
                        width: 100%;

                        .contact-details-left {
                            text-align: center;
                            width: 100%;
                        }
                    }

                    .contact-title {
                        padding-left: 0px;
                    }
                }
            }
        }

    }

    @media screen and (max-width: $xl) {

        .container-contact {

            .contact-hero {
                padding: 90px 0 90px 0;
            }
            
        }
    }



    @media screen and (max-width: $m) {

        .container-contact {

            .contact-hero {

                .contact-hero-left {

                    .contact-map {
                        width: 400px;
                        height: 300px;
                    }
                }

                .contact-hero-right {
                    
                    .contact-title {
                        font-size: 2em;
                    }

                    .contact-details {
                        font-size: 0.9em;
                    }

                }
            }
        }
    }

    @media screen and (max-width: $s) {

        .container-contact {

            .contact-hero {

                .contact-hero-left {

                    .contact-map {
                        width: 350px;
                        height: 262px;
                    }
                }
            }
        }
    }


</style>
