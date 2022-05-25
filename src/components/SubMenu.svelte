<script>
  import { handleClickMainMenu } from "./action.svelte";
  export let data;
</script>

<li class="sub-menu" on:click={handleClickMainMenu}>
  <a href="javascript:void(0);" name={data.childrenId}
    ><span>{data.title}</span><i
      class="arrow fa fa-angle-right pull-right"
    /></a
  >
</li>
