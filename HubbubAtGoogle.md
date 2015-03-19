# Introduction #

Here are all the potential places PubSubHubbub could be used in Google products and the current status, if any...

| **Product** | **Role** | **Status** | **Notes** |
|:------------|:---------|:-----------|:----------|
| Feedburner | pub | **95% done** | All burned feeds with PingShot enabled are now pinging the reference hub.  Few bugs are being ironed out, then we can call this 100% done. |
| Reader Shared Items | pub | <b><a href='http://googlereader.blogspot.com/2009/08/pubsubhubbub-support-for-reader-shared.html'>done</a></b> | (the Atom feed from e.g. http://www.google.com/reader/shared/bradfitz should ping a hub)  |
| Buzz | pub and sub | **done** | User feeds linked to your profile are subscribed using PSHB; output feeds are real-time |
| Blogger | pub | <b><b>95% done</b></b> | Live in production!  (need to add the discovery tag for RSS too, though...) |
| Google Alerts | pub | **done** | the Atom feeds that you can create from http://www.google.com/alerts; see [announcement post](http://googlecode.blogspot.com/2009/08/towards-programmable-web-pubsubhubbub.html) |
| Google Fast Flip | pub | **done** | The feeds are auto-discoverable for each category, e.g., [Business](http://fastflip.googlelabs.com/search?q=section:"Business") |
| Google Reader | sub | **done** | Feeds are received in real-time, but the UI does not update with Comet |
| Blog Search | sub | .. | obvious candidate |
| Google Code Project Hosting | pub | .. | all activity feeds on the site should ping |
| Latitude | pub | .. | Currently people with public location can have a JSON or KML file with the Latitude/Longitude.  Why not Atom/RSS with GeoRSS markup & pinging a hub? |
| Jaiku | pub,sub | .. | Jaiku updates would publish Hubbub events. Jaiku could also use Hubbub to enable life-streaming capabilities |
| YouTube | pub | .. | uploads, favorites, etc... |
| PicasaWeb | pub | .. | new photos (is there an Atom feed?) |