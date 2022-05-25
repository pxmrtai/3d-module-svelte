<script>

import { handleClickItemMenu } from "../action.svelte";

</script>
<li class="sub-menu-with-tool" id="art-word-menu">
  <a id="art-word" href="javascript:void(0);" class="header-sub-menu" name='art-word-menu'on:click={handleClickItemMenu}
    ><span>Art word</span><i class="arrow fa fa-angle-right pull-right" /></a
  >
  <ul>
    <li id="art-word-add">
      <div id="">
        <div class="text">Background color :</div>
        <input
          id="colorPickerArtWord"
          class="text-color-picker"
          type="color"
          value="#ffffff"
        />
      </div>
      <div class="text-input">
        <input type="text" id="text-input-art-word" />
        <button id="addTextArtWord">Add text</button>
      </div>
      <div id="artWordContainer">
        <canvas id="canvas2" style="border: 1px solid black; height: 500px" />
        <button id="apply">ok</button>
      </div>
    </li>
  </ul>
</li>
