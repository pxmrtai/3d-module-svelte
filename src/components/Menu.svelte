<script>
  import SubMenu from "./SubMenu.svelte";
  import BackgroundColor from "./ToolbarMenu/BackgroundColor.svelte";
  import Images from "./ToolbarMenu/Images.svelte";
  import Text from "./ToolbarMenu/Text.svelte";
  import ArtWord from "./ToolbarMenu/ArtWord.svelte";
import { menuValue } from "../constant/main.svelte";
</script>

<div class="tool-menu" id="tool-menu">
  <BackgroundColor />
  <Images />
  <Text />
  <ArtWord />
  <aside class="sidebar" id="sidebar">
    <div id="leftside-navigation" class="nano">
      <ul class="nano-content">
        {#each menuValue as item}
          <SubMenu data={item} />
        {/each}
      </ul>
    </div>
  </aside>
</div>
