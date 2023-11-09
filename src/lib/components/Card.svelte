<script>
export let myTitle;
export let myDescription;
export let myImage;
export let myLink;
// export let visible = true;
</script>


<div class="card">
  <h3>{myTitle}</h3>
  <a href="{myLink}">
    <img src="{myImage}" alt ="random">
    <p>{myDescription}</p>
  </a>
</div>

<style>
  .card {
  background-color: rgba(3, 117, 47, 0.74);
  text-align: center;
  margin:auto;

  height: 500px;
  width: 600px;

  border: 2rem;
  padding: 2px;
  border-radius: 5px;
  margin-top: 20px;
}
</style>








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