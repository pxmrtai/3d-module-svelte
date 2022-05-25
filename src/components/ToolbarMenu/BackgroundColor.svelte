<script>
  import { handleClickItemMenu } from "../action.svelte";
</script>

<li class="sub-menu-with-tool" id="background-color-menu" >
  <a
    id="background"
    href="javascript:void(0);"
    class="header-sub-menu"
    name='background-color-menu'
    on:click={handleClickItemMenu}
    ><span>Background Color</span><i
      class="arrow fa fa-angle-right pull-right"
    /></a
  >
  <ul>
    <li class="background-picker">
      <div class="text">Color:</div>
      <div class="color-input-container">
        <input id="colorPicker" type="color" value="#ffffff" />
      </div>
    </li>
  </ul>
</li>
