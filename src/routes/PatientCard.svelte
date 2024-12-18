<script>
  import test from '$lib/assets/test.webp'

  let {
    name = 'patient name',
    mr = 'medical records number',
    info = 'patient info',
    photo = {test}
  } = $props();
  

</script>

<div id="container">
  <p>MR: {mr}</p>
  <img src={photo} alt="patient">
  <h3>{name}</h3>
  <p>{info}</p>
</div>

<style>
  #container {
  	border: 1px solid black;
    width: 12rem;
    text-align: center;
  }

  img {
    width: 12rem;
  }
</style>
