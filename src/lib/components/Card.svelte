<script>
export let myTitle;
export let myDescription;
export let myImage;
export let myLink;
export let visible = true;
</script>

<!-- <h2>Testing Card Title</h2> -->

<!-- <h3>{cardTitle}</h3>
<p>{cardDescription}</p> -->

{#if visible = true}
<h3>{myTitle}</h3>
<a href="{myLink}">
<img src="{myImage}" alt ="random">
<p>{myDescription}</p>
</a>
{/if}








<!-- Different Solution -->

<!-- <div class ="card">
  <slot></slot>
</div>

<style>
  .card{
    background: white;
    padding: 20px;
    border-radius: 6px;
    box-shadow: 0px 2px 4px rgba(0,0,0,0.1);
  }
</style> -->