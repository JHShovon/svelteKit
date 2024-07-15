<script>
export let productID = 100;
</script>

<a href="/">Home</a>

<h1> Product List</h1>
<h1> <a href="/products/1">Product 1</a> </h1>
<h1> <a href="/products/2">Product 2</a> </h1>
<h1> <a href="{`/products/${productID}`}">{productID}</a> </h1>
