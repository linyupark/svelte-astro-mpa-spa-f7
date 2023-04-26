<Page>
  <h1>Index Svelte</h1>
  {JSON.stringify(f7route)}
  <ul>
    <li><Link href="/f7/about">About</Link></li>
  </ul>
</Page>

<script>
  import { Page, Link } from "framework7-svelte"
  export let f7route
  export let f7router
</script>