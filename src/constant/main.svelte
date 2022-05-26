<script context="module">
  import BackgroundColor from "../components/ToolbarMenu/BackgroundColor.svelte";
  import Images from "../components/ToolbarMenu/Images.svelte";
  import Text from "../components/ToolbarMenu/Text.svelte";
  import ArtWord from "../components/ToolbarMenu/ArtWord.svelte";

  export const menuValue = [
    {
      childrenId: "background-color-menu",
      title: "Background Color",
      content: BackgroundColor,
    },
    {
      childrenId: "images-menu",
      title: "Images",
      content: Images,
    },
    {
      childrenId: "text-number-menu",
      title: "Text & Number",
      content: Text,
    },
    {
      childrenId: "art-word-menu",
      title: "Art Word",
      content: ArtWord,
    },
  ];
  export const tshirtParts = [
    { label: "Front", value: "front" },
    { label: "Back", value: "back" },
    { label: "Neck", value: "neck" },
    { label: "Left Hand", value: "left-hand" },
    { label: "Right Hand", value: "right-hand" },
  ];
</script>
