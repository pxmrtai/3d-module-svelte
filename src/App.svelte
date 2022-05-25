<script>
  import "./css/main.css";
  import RadioModulePart from "./components/RadioModulePart.svelte";
  import Menu from "./components/Menu.svelte";
  import { tshirtParts } from "./constant/main.svelte";
</script>

<div class="container">
  <div class="dialog-container">
    <div class="radio-group">
      {#each tshirtParts as tshirtPart}
        <RadioModulePart {tshirtPart} />
      {/each}
    </div>
    <div class="row-content">
      <Menu />
      <div class="two-d" id="2d" />
      <div class="three-d" id="3d" />
    </div>
    <div class="button-group">
      <button class="btn btn-save" id="confirmPreview">CONFIRM PREVIEW</button>
    </div>
  </div>
</div>

<style>
</style>
