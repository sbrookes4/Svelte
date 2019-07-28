<script>
	import Product from './Product.svelte';
	import Navbar from './Navbar.svelte';
	import Banner from './Banner.svelte';

	let name = 'Your';
	let name1 = 'Products'; 
	let title= '';
	let price = 0;
	let info = '';
	let button = '';

	function setTitle(event){
		title = event.target.value;
	}

	function setPrice(event){
		price = event.target.value;
	}

	function setInfo(event){
		info = event.target.value;
	}

	function setButton(event){
		info = event.target.value;
	}

</script>

<style>

.mook{
color:greenyellow;
}

section{
	margin: 1rem;
    padding: 1rem;
	box-shadow: 0 2px 8px rgba(0, 0, 0, .26);
}

</style>

<Banner />


<h1 class="mook">Hello Moo. {name} {name1}!!!</h1>

<Navbar />

<section>

<div>

<h1>Add Product </h1>
<label>Title</label><br>
<input type="text" value={title} on:input="{setTitle}"><br><br>
</div>

<div>
<label>Price</label><br>
<input type="number" bind:value={price}><br><br>
</div>

<div>
<label>Information</label><br>
<textarea name="" id="descriotion" row="10" bind:value={info}></textarea>
</div>

<div>
<label>Button Text</label><br>
<input type="text" value={button} on:input="{setButton}"><br><br>
</div>

</section>

<Product 
productTitle={title} 
productPrice={price} 
productInfo={info} />





