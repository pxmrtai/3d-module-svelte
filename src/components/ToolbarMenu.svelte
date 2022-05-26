<script>
  import { handleClickItemMenu } from "./action.svelte";
  export let data;
</script>

<li class="sub-menu-with-tool" id={data.childrenId} style="right: -2000px">
  <a
    class="header-sub-menu"
    name={data.childrenId}
    on:click={handleClickItemMenu}
    ><span name={data.childrenId}>{data.title}</span><i
      name={data.childrenId}
      class="arrow fa fa-angle-right pull-right"
    /></a
  >
  <slot />
</li>
