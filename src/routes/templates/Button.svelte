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
        transition: all 0.3s ease-in-out;

        &:hover {
            background-color: $text;
            color: $secondary;
            transform: scale(1.05);
        }
    
    }

    @media screen and (max-width: $xl) {
        .btn {
            height: 35px;
            font-size: 0.9em;
        }
    }

</style>