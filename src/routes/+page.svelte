<script>
import {
    goto,
    beforeNavigate,
    afterNavigate
} from "$app/navigation";
const handleClick = () => {
    console.log('Placing your order');
    goto('/products')
}

beforeNavigate((navigation) => {
    console.log({
        before: navigation
    });
})
afterNavigate((navigation) => {
    console.log({
        after: navigation
    });
})
</script>
<h1>Home page</h1>

<ul>
    <li><a href="/">Home</a></li>
    <li><a href="/blog">blog</a></li>
    <li><a href="/products">products</a></li>
</ul>

<button on:click={handleClick}>Place order</button>
