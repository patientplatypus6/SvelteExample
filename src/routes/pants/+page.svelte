
<script>
  import { getContext } from 'svelte';
  
  const name = getContext('name');
  const changeName = getContext('changeName');
  // Retrieve user store from context  const user = getContext('user');
</script>

<div class="main">
  <p>Welcome {$name}</p>

  <input on:input={evt => {changeName(evt.target.value)}}/>

  <h1>About this site</h1>
  <p>TODO...</p>
  <a href="/">Home</a>
</div>