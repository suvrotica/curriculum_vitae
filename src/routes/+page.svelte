<script>
    import SectionHeader from "../lib/components/SectionHeader.svelte";
</script>

<main class="container">
    <table>
        <tbody>
            <tr>
                <td>
                    <SectionHeader
                        leftText="Post Graduate - University of Texas at San Antonio<i>San Antonio, Texas, USA</i>"
                        rightText="Cum Laude <b>1998-2000</b>"
                    />
                </td>
            </tr>
            <tr>
                <td>
                    <SectionHeader
                        leftText="Graduate - Jadavpur University <i>Jadavpur,Kolkata, WB, India</i>"
                        rightText="First Class <b>1994-1998</b>"
                    />
                </td>
            </tr>
            <tr>
                <td>
                    <SectionHeader
                        leftText="College - St. Xaviers <i>Park Street, Kolkata, WB, India</i>"
                        rightText="Marks 80% <b>1992-1994</b>"
                    />
                </td>
            </tr>
            <tr>
                <td>
                    <SectionHeader
                        leftText="School - WWA Cossipore English School <i>Dum Dum, Kolkata, WB, India</i>"
                        rightText="Marks 93% <b>1982-1992</b>"
                    />
                </td>
            </tr>
        </tbody>
    </table>
</main>

<style>
    main {
        margin: auto;
		width: 95%;
    }
</style>