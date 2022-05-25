<script>

import { handleClickItemMenu } from "../action.svelte";

</script>
<li class="sub-menu-with-tool" id="text-number-menu">
    <a id="text-number" href="javascript:void(0);" class="header-sub-menu" name="text-number-menu" on:click={handleClickItemMenu}
      ><span>Text & Number</span><i
        class="arrow fa fa-angle-right pull-right"
      /></a
    >
    <ul>
      <li id="text-edit-add">
        <div class="text-input">
          <div class="btn add-button" id="addText">
            <i class="fa-solid fa-plus" />
          </div>
        </div>
      </li>
    </ul>
  </li>