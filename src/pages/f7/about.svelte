<script>
  import { Page, Link, Navbar, Block } from "framework7-svelte";
  export let f7route;
  export let f7router;
</script>

<Page>
  <Navbar title="asdasd" backLink=" " />
  <Block>
    About
    <a
      href
      on:click={() => {
        location.href = "/f7/profile/help-center";
      }}>硬跳转到独立页面</a
    >
  </Block>
</Page>
