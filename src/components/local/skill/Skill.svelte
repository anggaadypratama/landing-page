<script>
    import Deskripsi from '../../Deskripsi.svelte'

    export let className = ""

    const desc = {
        judul : 'Skill & Experience',
        desc:  `The main area of my expertise in front end development 
                (client side of web). <br/> <br/>

                HTML, CSS, SCSS, LESS, JavaScript, Node.js, Json, Rest Api,
                React, Svelte.js, Progresive Web Apps, Dart, Flutter, and
                React Native. <br/> <br/>

                I have also UI/UX experience with Photoshop, Ilustrator, 
                Figma and adobe XD.`
	}
</script>

<div class="wrapper {className}">
    <Deskripsi className="absolute m-0 top-0 transform translate-y-1/2" judul={desc.judul} deskripsi={desc.desc}/>
</div>


<style lang="scss">
    @import '../../../../static/style/global.scss';

    .wrapper{
        height: 100%;
        width: 80%;
        margin-left: 5%;
    }
</style>