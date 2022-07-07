<html>
	<script>
		Notification.requestPermission().then( function ( permission ) {
			
			console.log( 'Inside Request Permission' );
			
			if ( permission === "granted" ) {
				
				console.log( 'Inside Granted Permission' );
				const sampleNotification = new Notification( 'Sample Title' );

				sampleNotification.onclick = () => {
					console.log( 'Notification clicked' );
				}

			}
		} );
	</script>
</html>
