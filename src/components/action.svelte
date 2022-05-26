<script context="module">
  export function handleClickMainMenu(e) {
    const sidebar = document.getElementById("sidebar");
    let childrenId;
    if (e.target.name) {
      childrenId = document.getElementById(e.target.name);
    } else {
      childrenId = document.getElementById(e.target.getAttribute("name"));
    }
    sidebar.style.left = "-2000px";
    childrenId.style.right = "0";
  }
  export function handleClickItemMenu(e) {
    const sidebar = document.getElementById("sidebar");
    let childrenId;
    if (e.target.name) {
      childrenId = document.getElementById(e.target.name);
    } else {
      childrenId = document.getElementById(e.target.getAttribute("name"));
    }
    sidebar.style.left = "0";
    childrenId.style.right = "-2000px";
  }
</script>
