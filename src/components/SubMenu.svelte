<script>
  import { handleClickMainMenu } from "./action.svelte";
  export let data;
</script>

<li class="sub-menu" on:click={handleClickMainMenu}>
  <a href="javascript:void(0);" name={data.childrenId}
    ><span name={data.childrenId}>{data.title}</span><i
      name={data.childrenId}
      class="arrow fa fa-angle-right pull-right"
    /></a
  >
</li>
