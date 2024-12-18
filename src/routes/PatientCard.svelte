<script>
  import test from '$lib/assets/test.webp'
  import { patients } from '$lib/patients.js'

  let {
    name = 'patient name',
    mr = 'medical records number',
    info = 'patient info',
    photo = {test},
    link = '#'
  } = $props();
  

</script>

<div id="container">
  <a href={link}>
    <p>MR: {mr}</p>
    <img src={photo} alt="patient">
    <h3>{name}</h3>
    <p>{info}</p>
  </a>
</div>

<style>
  #container {
  	border: 1px solid black;
    width: 12rem;
    text-align: center;
    cursor: pointer;
  }

  #container a {
    text-decoration: none;
  }
 
  img {
    width: 12rem;
  }
</style>
