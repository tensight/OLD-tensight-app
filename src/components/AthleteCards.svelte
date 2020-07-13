<script>
    const QUERY = `
		query {
			athletes {
				id
                firstName
                lastName
                sport
                currently
			}
		}
	`;
	const QUERYRES = {};
    
    import TailwindCSS from "./TailwindCSS.svelte";
</script>

{JSON.stringify(QUERYRES)}
<!-- {#each QUERYRES.athletes as athlete}
<div>
    <img src="" alt="alt-text">
    <div class="p-6">
        <h4>{`${athlete.firstName} ${athlete.lastName}`}</h4>
        <div>
            {athlete.sport}
        </div>
        <div>
            Currently {athlete.currently}
        </div>
    </div>
</div>
{/each} -->