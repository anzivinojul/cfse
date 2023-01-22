<button class="btn">{textButton}</button>

<script lang="ts">
    export let textButton:string
</script>

<style lang="scss">

    @import '../../app.scss';

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
</style>