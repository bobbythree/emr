<script>
  import { patients } from '$lib/patients';
  import { page } from '$app/stores';
  const routeName = $page.url.pathname.slice(1);
</script>

{#each patients as patient}
  {#if patient.mr == routeName}
  <h1>{patient.name}</h1>    
  {/if}
{/each}

<style>
    h1 {
        text-align: center;
    }
</style>