<script>
	import RibbonToolbar from './ui/RibbonToolbar.svelte';
	import Login from "./pages/Login.svelte";
	import Ticket from './pages/Ticket.svelte';
	import DatePicker from './ui/DatePicker.svelte';
	let url = "https://gis.lrgvdc911.org/php/spartan/api/v2/index.php/";
	const socket = io('http://localhost:3000');
	
	socket.on('connect', () => {
		
	});
</script>


<!-- <DatePicker /> -->
<!-- <Login /> -->

<RibbonToolbar {socket} url={url} />
<!-- <Ticket /> -->