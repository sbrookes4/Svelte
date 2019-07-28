<script>

export let productTitle;
export let productPrice;
export let productInfo;


</script>

<style >

div{
    margin: 1rem;
    padding: 1rem;
    box-shadow: 0 2px 8px rgba(0, 0, 0, .26);
    border-radius:5px;
    background-color: white;
}

h1{
    font-size: 1.25rem;
    margin: 0.25rem 0;
}

h2{
    color: green;
    font-size: 1rem;
    margin: 0.25rem 0;
}

p{
    margin: 0.25rem .25rem;   
}

button{
    font:inherit;
    padding:.15rem;
    border:2px solid rgb(0, 0, 0);
    color:white;
    background:rgb(128, 127, 127);
    cursor: pointer;
}

button:hover{
box-shadow: 0 2px 8px rgba(0, 0, 0, .26); 
}

</style>

<div>

<h1>{productTitle}</h1>
<h2>{productPrice}</h2>
<p >{productInfo}</p>
<button></button>


</div>