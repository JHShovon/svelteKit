<script>
	import { page } from '$app/stores';
    const grettings = {
        en : "Hello",
        es : "Hola",
        bn: "ওহে"
    }

    const {lang = 'en'} = $page.params
    
    const gretting = grettings[lang]
    console.log(gretting);
</script>

<h1>{gretting}</h1>