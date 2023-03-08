
<style>
  /* this div is a component that takes specific styling */
  .styleddiv{
    color: red;
    background: black;
    margin: 10px;
    font-size: 20px;
    text-align: center;
    font-weight: bold;
    padding: 20px;
    border-radius: 5px;
    width: 20vw;
  }
</style>

<script>
    export let toggle = () => {} // no-operation function
</script>

<div class='styleddiv'> 
  This div should be styled
  <button on:click={toggle(22)}>~Click Me~</button>
</div>