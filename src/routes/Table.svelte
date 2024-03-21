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
			amount: "860,000",
			currency: '$'
		},
		{
			name: 'Danie Du Toit',
			status: 'Not Yet Claimed',
			country: 'South Africa',
			amount: "950,000",
			currency: 'R'
		},
		{
			name: 'Peter Frederick',
			status: 'Not Yet Claimed',
			country: 'South Africa',
			amount: "2,450,000",
			currency: 'ZAR'
		},
		{
			name: 'Cathy Lorne Conklin',
			status: 'Claimed',
			country: 'South Africa',
			amount: '350,000',
			currency: '$'
		},
		{
			name: 'Rina Van derrick',
			status: 'Claimed',
			country: 'South Africa',
			amount: "2,790,000",
			currency: 'ZAR'
		},
		{
			name: 'Laetitia Posthumus Brand',
			status: 'Claimed',
			country: 'South Africa',
			amount: "2,570,000",
			currency: 'ZAR'
		},
		{
			name: 'Barend Frederik Hendrik',
			status: 'Not Yet Claimed',
			country: 'South Africa',
			amount: "3,370,000",
			currency: 'ZAR'
		},
		{
			name: 'Willbard Van Wyk Ardeas',
			status: 'Not Yet Claimed',
			country: 'South Africa',
			amount: "2,350,000",
			currency: 'NAD'
		},
		{
			name: 'Alet Botha',
			status: 'Claimed',
			country: 'South Africa',
			amount: "3,830,000",
			currency: 'ZAR'
		},
		{
			name: 'Gesie Van Zyl',
			status: 'Claimed',
			country: 'South Africa',
			amount: "3,830,000",
			currency: 'NAD'
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
				<TableBodyCell>
					<div
						class={`${winner.status === 'Claimed'
							? 'bg-green-400 rounded-full px-2'
							: 'bg-red-500 rounded-full px-2'} text-center text-white`}
					>
						{winner.status}
					</div>
				</TableBodyCell>
				<TableBodyCell>{winner.country}</TableBodyCell>
				<TableBodyCell>{winner.currency}{winner.amount}</TableBodyCell>
			</TableBodyRow>
		{/each}
	</TableBody>
</Table>
