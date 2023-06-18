<script>
  export let links;
</script>

<nav>
  <ul>
    <li>
      <img src="/Images/Logo.jpg" alt="logo" width="50%" />
    </li>
  </ul>
  <ul>
    {#each links as link}
      <li>
        <a href={link.href} title={link.title}>{@html link.title}</a>
      </li>
    {/each}
  </ul>
</nav>

<style>
  strong {
    text-transform: uppercase;
  }
  nav {
    margin: auto;
    width: 95%;
  }

  a {
    text-transform: lowercase;
    text-decoration: none;
  }
</style>
