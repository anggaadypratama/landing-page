
<script>
    export let target = '.'
    export let background = ''
    export let textColor = ''
    export let className = ''
</script>

<a class="costum-button {className}" style="background-color: {background}; color: {textColor};" lang="scss" href={target}>
    <slot></slot>
</a>

<style lang="scss">
    @import '../../static/style/global.scss';

    .costum-button{
        padding: 11px 28px;
        border-radius: 5px;
        font-family: $viga;

        @media screen and (max-width: $lg - 1) and (min-width: $md){
            width: 100%;
            text-align: center;
        }

        @media screen and (max-width: $sm - 1){
            width: 100%;
            text-align: center;
            margin-top: 1rem;
        }

        &:hover{
            transition: .3s ease-in-out;
            opacity: .9;
        }

    }
</style>