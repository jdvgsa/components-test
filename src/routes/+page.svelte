<script> 
import Card from "../lib/components/Card.svelte";
import {cardData} from "../lib/data.js"
import {cardArray} from "../lib/data.js"
// renders card
// let visible = true;
</script>
<head>
<style>

h1 {
  display: flex;
  justify-content: center;
}

nav {
  
  display: flex;
  justify-content: space-evenly;
  background-color: transparent;
  list-style: none;
  padding-bottom: 2rem;
  padding-top: 0;
  text-decoration: underline;
  background-color: antiquewhite;
  color: antiquewhite;

  text-rendering: optimizeLegibility;
  text-shadow: 1px 1px 1px rgba(0, 0, 0, 0.8);
}

nav a {
  color: grey;
  text-decoration: none;
  margin-right: 1rem;
}

nav a:hover {
  text-decoration:underline;
  color: red;

}

/* .card {
  background-color: rgba(3, 117, 47, 0.74);
  text-align: center;
  margin:auto;

  height: 500px;
  width: 600px;

  border: 2rem;
  padding: 2px;
  border-radius: 5px;
  margin-top: 20px;
} */

footer {
  position: fixed;
  bottom: 0;
  background-color: rebeccapurple;
  color: rgba(255, 255, 255, 0.938);
  text-align: center;
  padding: .25rem;
  width: 100%;

}


</style>
</head>

   <nav>
    
      <li> <a href="/">Home</a></li>
      <li> <a href="/about">About</a></li>
      <li> <a href="/contact">Contact</a></li>
    
  </nav>
  

<h1 class="text-5xl font-bold underline">Components and Props Assignment Test</h1>

<div class="card">
<Card {...cardData}/>
</div>

<h1>My cardArray</h1>
<span>

{#each cardArray as card}
<Card {...card}/>
{/each}

</span>
<p><br></p>
<p><br></p>
<footer><p>&copy; 2023 John Dagsa Svelte Assignment</p></footer>

