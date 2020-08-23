<script>
    import Deskripsi from '../../Deskripsi.svelte'
    import Button from '../../Button.svelte'
    import style from '../../../../static/style/style'

    const { Color } = style

    export let className = ""

    const desc = {
        judul : 'Front end developer and UI/UX Designer.',
        desc: `As a creative person I love learning something new to 
        get alternative solutions for various problems.
        Creativity really helped me in motivate myself to continue 
        forward to my goal wan achieved.`
	}
</script>

<div class="wrapper {className}">
    <Deskripsi className="absolute m-0 top-0 transform translate-y-1/2" judul={desc.judul} deskripsi={desc.desc}>
        <h2>Hi I'm Angga Ady Pratama</h2>
        <div slot="child" class="mt-12 flex flex-wrap">
            <Button target="mailto:anggaadypratama@outlook.com" className="mr-4" background={Color.secondary} textColor={Color.white}>Email Me</Button>
            <Button className="mt-0 md:mt-4 lg:mt-0" background={Color.transparent} textColor={Color.text}>Download Resume</Button>
        </div>
    </Deskripsi>
</div>

<style lang="scss">
    @import '../../../../static/style/global.scss';

    .wrapper{
        height: 100%;
        width: 80%;
        margin-left: 5%;
        
    }

    h2{
        font-family: $viga;
        color: $secondary;
    }
</style>