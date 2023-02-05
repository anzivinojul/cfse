<button class="btn" on:click={goTo('.container-contact')} on:keypress={goTo('.container-contact')}>{textButton}</button>

<script lang="ts">
    export let textButton:string

    function getHeaderHeight(): number {
        const header = document.querySelector('#header');
        const height = header!.getBoundingClientRect().height;

        return height;
    }

    const goTo = (container: string) => () => {
        const containerDOM = document.querySelector(container);
        const height = (containerDOM!.getBoundingClientRect().top + window.scrollY) - getHeaderHeight();

        window.scrollTo(
            {
                top: height,
                left: 0,
                behavior: "smooth"
            }
        );
    }

</script>

<style global lang="scss">

    .btn {
        display: flex;
        justify-content: center;
        cursor: pointer;
        font-family: $font_opensans;
        font-weight: bold;
        font-size: 1em;
        border: 3px solid transparent;
        display: inline-flex;
        height: 40px;
        padding: 0 space(4);
        border-radius: 30px;
        align-items: center;
        color: $text;
        background-color: $secondary;
        transition: .4s;

        &:hover {
            background-color: lighten($secondary, 5%);
            border: 3px solid $text;
        }
    
    }

    @media screen and (max-width: $xl) {
        .btn {
            height: 35px;
            font-size: 0.9em;
            padding: 0 space(2);
        }
    }

</style>