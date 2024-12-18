<script>
  import PatientCard from './PatientCard.svelte';
  import test from '$lib/assets/test.webp';
  import { patients } from '$lib/patients.js';
  
</script>
  

<div id="container">
  {#each patients as patient}
    <PatientCard name = {patient.name} mr = {patient.mr} photo = {test} info = {patient.info} />
    
  {/each}

</div>

<style>
  #container {
    display: flex;
    gap: 0.5rem;
  }
</style>
