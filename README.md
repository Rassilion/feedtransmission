# feedtransmission
feedtransmission is a python script to read RSS/Atom feeds of torrents and add them to Transmission to download

## Usage

```
feedtransmission.py http://url.to/torrent/feed.xml http://another.url/to/feed
```

Most probably you want to add feedtransmission to your cron file to regularly monitor a feed.

List of parameters available:
```
  --transmission-host <host>
                        Host for Transmission RPC (default: localhost)
  --transmission-port <port>
                        Port for Transmission RPC (default: 9091)
  --transmission-user <user>
                        Port for Transmission RPC (default: None)
  --transmission-password <password>
                        Port for Transmission RPC (default: None)
  --log-file <logfile path>
                        The logging file, if not specified, prints to output
  --clear-added-items   Clears the list of added torrents. You can also do
                        that by deleting the addeditems.txt
  --download-dir <dir>  The directory where the downloaded contents will be
                        saved in. Optional.
```


The script makes a file called `addeditems.txt` in the folder of the executable. This file stores the torrent links already added to Transmission.
