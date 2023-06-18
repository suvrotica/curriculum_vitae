<!-- SectionHeader.svelte -->
<script>
  export let leftContent;
  export let rightContent;
</script>

<div>
  <nav>
    <ul>
      <li><slot name="leftContent">{leftContent}</slot></li>
    </ul>
    <ul>
      <li><slot name="rightContent">{rightContent}</slot></li>
    </ul>
  </nav>
</div>
