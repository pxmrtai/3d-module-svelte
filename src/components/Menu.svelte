<script>
  import SubMenu from "./SubMenu.svelte";
  import BackgroundColor from "./ToolbarMenu/BackgroundColor.svelte";
  import Images from "./ToolbarMenu/Images.svelte";
  import Text from "./ToolbarMenu/Text.svelte";
  import ArtWord from "./ToolbarMenu/ArtWord.svelte";
  import { menuValue } from "../constant/main.svelte";
  import ToolbarMenu from "./ToolbarMenu.svelte";
</script>

<div class="tool-menu" id="tool-menu">
  <aside class="sidebar" id="sidebar">
    <div id="leftside-navigation" class="nano">
      <ul class="nano-content">
        {#each menuValue as item}
          <SubMenu data={item} />
        {/each}
      </ul>
    </div>
  </aside>
  {#each menuValue as item}
    <ToolbarMenu data={item}>
      {#if item.content}
        <svelte:component this={item.content} />
      {:else}
        not thing
      {/if}
    </ToolbarMenu>
  {/each}
</div>
