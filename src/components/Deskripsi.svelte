<script>
    export let judul = 'Judul';
    export let deskripsi = 'Deskripsi';
    export let className = ''
</script>

<div class="{className}">
    <slot></slot>

    <h1>
        {judul}
    </h1>
    <p>
        {@html deskripsi}
    </p>

    <slot name="child"></slot>
</div>

<style lang="scss">
    @import '../../static/style/global.scss';

    h1{
        font-family: $viga;
        color: $white;
    }

    p{
        margin-top: 10px;
        font-family: $roboto;
        color: $text;
    }
</style>