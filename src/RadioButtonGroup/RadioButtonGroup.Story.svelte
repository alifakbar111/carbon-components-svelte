<script>
  import RadioButtonGroup from "./RadioButtonGroup.svelte";
  import { RadioButton } from "../RadioButton";
  import { FormGroup } from "../FormGroup";

  $: selected = "default-selected";
</script>

<FormGroup legendText="Radio Button heading">
  <RadioButtonGroup {...$$props.group} legend="Group Legend" bind:selected>
    <RadioButton {...$$props.radio} value="standard" id="radio-1" />
    <RadioButton {...$$props.radio} value="default-selected" id="radio-2" />
    <RadioButton {...$$props.radio} value="disabled" id="radio-3" />
  </RadioButtonGroup>
</FormGroup>
