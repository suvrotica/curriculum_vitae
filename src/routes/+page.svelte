<script>
    import SectionHeader from "../lib/components/SectionHeader.svelte";
    import Education from "../lib/components/Education.svelte";
    let phone_icon_image= "/Images/phone.svg";
    let education_list = [
        {
            stage: "Post Graduate (MS)",
            name: "University of Texas at San Antonio",
            address: "One UTSA Circle, San Antonio, TX 78249, USA",
            phone: "+1-210-458-4011",
            href: "www.utsa.edu",
            marks: "Cum Laude ",
            years: "1998-2000",
        },
        {
            stage: "Graduate (BCSE)",
            name: "Jadavpur University",
            address:
                "188, Raja Subodh Chandra Mallick Rd, Jadavpur, Kolkata, West Bengal 700032, India",
            phone: "+91-33-2457-2227",
            href: "www.jaduniv.edu.in",
            marks: "First Class ",
            years: "1994-1998",
        },
        {
            stage: "College",
            name: "St. Xaviers",
            address:
                "30 Mother Teresa Sarani, Kolkata, West Bengal 700016, India",
            phone: "+91-33-22551171",
            href: "www.sxcsccu.edu.in",
            marks: "First Division 80% ",
            years: "1992-1994",
        },
        {
            stage: "School",
            name: "WWA Cossipore English School",
            address: "4, Dum Dum Road, Seven Tanks Ln, Kolkata, 700002, India",
            phone: "+91-33-2557-4373",
            href: "wwaces.in/v2/",
            marks: "ICSE School First 93% ",
            years: "1982-1992",
        },
    ];
</script>



<main class="container">
    <Education {education_list} {phone_icon_image}/>
</main>

<style>
    main {
        margin: auto;
		width: 95%;
    }
</style>