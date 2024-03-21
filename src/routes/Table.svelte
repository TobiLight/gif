<script>
	import {
		Table,
		TableBody,
		TableBodyCell,
		TableBodyRow,
		TableHead,
		TableHeadCell
	} from 'flowbite-svelte';
	const winners = [
		{
			name: 'Koekie Fergueson',
			status: 'Claimed',
			country: 'USA',
			amount: 860000,
      currency: "$"
		},
    {
      name: 'Danie Du Toit',
			status: 'Not Yet Claimed',
			country: 'South Africa',
			amount: 950000,
      currency: "R"
    },
    {
      name: 'Peter Frederick ',
			status: 'Not Yet Claimed',
			country: 'South Africa',
			amount: 2450000,
      currency: "ZAR"
    }
	];
</script>

<Table striped={true}>
	<TableHead>
		<TableHeadCell>Name</TableHeadCell>
		<TableHeadCell>Status</TableHeadCell>
		<TableHeadCell>Country</TableHeadCell>
		<TableHeadCell>Amount</TableHeadCell>
		<!-- <TableHeadCell>
      <span class="sr-only">Edit</span>
    </TableHeadCell> -->
	</TableHead>
	<TableBody tableBodyClass="divide-y">
		{#each winners as winner}
			<TableBodyRow>
				<TableBodyCell>{winner.name}</TableBodyCell>
				<TableBodyCell>{winner.status}</TableBodyCell>
				<TableBodyCell>{winner.country}</TableBodyCell>
				<TableBodyCell>{winner.currency}{winner.amount}</TableBodyCell>
			</TableBodyRow>
		{/each}
	</TableBody>
</Table>
