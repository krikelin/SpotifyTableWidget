# Spotify TableView

Table view for Spotify Apps

![Table widget](http://img402.imageshack.us/img402/4105/widgetw.png)

# Usage

script.js (or equivalent)

				// Creates a playlist with sortable table.
				var table = sp.require("sp://<your_app>/<path>/<to>/<table-folder>/table");
				console.log(playlist);
				var list = new table.Table(playlist, function(track) {
				
					try {
						var track = new views.Track(track, views.Track.FIELD.SHARE| views.Track.FIELD.STAR| views.Track.FIELD.NAME | views.Track.FIELD.ARTIST | views.Track.FIELD.ALBUM | views.Track.FIELD.DURATION);
						
					//	console.log(track.track);
						var year = track.track.data.album.year;
							
						$(track.node).append("<span class=\"sp-track-field-year\"><a href=\"spotify:app:timemachine:year:" + year + ":" + year + ":" + params + "			\">" + year + "</a></span>");

			
					try {
						var track = new views.Track(track, views.Track.FIELD.SHARE| views.Track.FIELD.STAR| views.Track.FIELD.NAME | views.Track.FIELD.ARTIST | views.Track.FIELD.ALBUM | views.Track.FIELD.DURATION);
						
						//	console.log(track.track);
						var year = track.track.data.album.year;
						
							$(track.node).append("<span class=\"sp-track-field-year\"><a href=\"spotify:app:timemachine:year:" + year + ":" + year + ":" + params + "			\">" + year + "</a></span>");

						return track;
					} catch (e) {
						console.log(e.stack);
					}
				});
				} catch(e) {
					console.log(e.stack);
				}