# Spotify TableView
<<<<<<< HEAD
Table view for Spotify Apps

# Usage

=======
No newline at end of file
# Spotify TableView
Table view for Spotify Apps

# Usage
 
>>>>>>> New entry
script.js (or equivalent)

				// Creates a playlist with sortable table.
				var table = sp.require("sp://<your_app>/<path>/<to>/<table-folder>/table");
				console.log(playlist);
				var list = new table.Table(playlist, function(track) {
<<<<<<< HEAD
				
					try {
						var track = new views.Track(track, views.Track.FIELD.SHARE| views.Track.FIELD.STAR| views.Track.FIELD.NAME | views.Track.FIELD.ARTIST | views.Track.FIELD.ALBUM | views.Track.FIELD.DURATION);
						
					//	console.log(track.track);
						var year = track.track.data.album.year;
							
						$(track.node).append("<span class=\"sp-track-field-year\"><a href=\"spotify:app:timemachine:year:" + year + ":" + year + ":" + params + "			\">" + year + "</a></span>");
=======
			
					try {
						var track = new views.Track(track, views.Track.FIELD.SHARE| views.Track.FIELD.STAR| views.Track.FIELD.NAME | views.Track.FIELD.ARTIST | views.Track.FIELD.ALBUM | views.Track.FIELD.DURATION);
						
						//	console.log(track.track);
						var year = track.track.data.album.year;
						
							$(track.node).append("<span class=\"sp-track-field-year\"><a href=\"spotify:app:timemachine:year:" + year + ":" + year + ":" + params + "			\">" + year + "</a></span>");
>>>>>>> New entry
						return track;
					} catch (e) {
						console.log(e.stack);
					}
				});
				} catch(e) {
					console.log(e.stack);
				}

index.html 

				<head>
				....
<<<<<<< HEAD
				<link rel="stylesheet" href="sp://<your_app>/<path>/<to>/<table-folder>/table.css" />
=======
					<link rel="stylesheet" href="sp://<your_app>/<path>/<to>/<table-folder>/table.css" />
>>>>>>> New entry
				....
				</head>
			

