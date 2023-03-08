<script>

  //this is where global context goes (i.e. context API)
  //for most applications a redux like pattern shouldn't be necessary
  //use context instead
  // the "slot" keyword is an injection syntax telling sveltekit to inject layout before page.svelte

  import { setContext } from 'svelte';
  import { writable } from 'svelte/store';

  let name = writable('John');
  const changeName = (value) => {
    $name = value;
  }

  setContext('changeName',changeName);
  setContext('name',name);
</script>



<slot />