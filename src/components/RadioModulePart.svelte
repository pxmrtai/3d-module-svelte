<script>
  export let tshirtPart;
</script>

<div class="radio-item">
  <label for={tshirtPart.label}>{tshirtPart.label}</label>
  <input
    type="radio"
    id={tshirtPart.label}
    name="t-shirt-part"
    value={tshirtPart.label}
  />
</div>
