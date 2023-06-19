<script>
  export let phone_icon_image;

  let education_list = [
    {
      stage: "Post Graduate (MS)",
      name: "University of Texas at San Antonio",
      address: "One UTSA Circle, San Antonio, TX 78249, USA",
      phone: "+1-210-458-4011",
      href: "http://www.utsa.edu",
      marks: "Cum Laude ",
      years: "1998-2000",
    },
    {
      stage: "Graduate (BCSE)",
      name: "Jadavpur University",
      address:
        "188, Raja Subodh Chandra Mallick Rd, Jadavpur, Kolkata, West Bengal 700032, India",
      phone: "+91-33-2457-2227",
      href: "http://jadavpuruniversity.in/",
      marks: "First Class ",
      years: "1994-1998",
    },
    {
      stage: "College (HS)",
      name: "St. Xaviers",
      address: "30 Mother Teresa Sarani, Kolkata, West Bengal 700016, India",
      phone: "+91-33-22551171",
      href: "http://www.sxcsccu.edu.in",
      marks: "First Division 80% ",
      years: "1992-1994",
    },
    {
      stage: "School (ICSE)",
      name: "WWA Cossipore English School",
      address: "4, Dum Dum Road, Seven Tanks Ln, Kolkata, 700002, India",
      phone: "+91-33-2557-4373",
      href: "http://wwaces.in/v2/",
      marks: "ICSE School First 93% ",
      years: "1982-1992",
    },
  ];
</script>

{#each education_list as level}
  <details>
    <summary>{level.stage} - {level.name}</summary>
    <nav>
      <ul>
        <li>{level.address}</li>
        <li>{level.phone}</li>
      </ul>
      <ul>
        <li>
          <span><a role="button" href={level.href}>URL</a></span>
        </li>
      </ul>
    </nav>
    <p>{level.marks}<b>{level.years}</b></p>
  </details>
{/each}

<style>
  summary {
    font-weight: 200;
  }
  li,
  p,
  a {
    font-weight: 200;
    font-size: medium;
  }
  li {
    font-weight: 200;
    font-size: small;
  }
</style>
