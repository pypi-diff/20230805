# Comparing `tmp/nyct-gtfs-1.2.0.tar.gz` & `tmp/nyct-gtfs-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nyct-gtfs-1.2.0.tar", last modified: Thu Dec  9 04:07:19 2021, max compression
+gzip compressed data, was "C:\Users\fortk\PycharmProjects\nyct-gtfs\dist\.tmp-8bbfin9f\nyct-gtfs-1.3.0.tar", last modified: Sat Aug  5 18:43:12 2023, max compression
```

## Comparing `nyct-gtfs-1.2.0.tar` & `nyct-gtfs-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-12-09 04:07:19.546069 nyct-gtfs-1.2.0/
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)     1094 2021-12-09 04:00:03.163165 nyct-gtfs-1.2.0/LICENSE.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)    13163 2021-12-09 04:07:19.539068 nyct-gtfs-1.2.0/PKG-INFO
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)    13011 2021-12-09 04:01:24.696412 nyct-gtfs-1.2.0/README.md
-drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-12-09 04:07:19.484589 nyct-gtfs-1.2.0/nyct_gtfs/
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)      185 2021-12-09 04:02:11.491432 nyct-gtfs-1.2.0/nyct_gtfs/__init__.py
-drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-12-09 04:07:19.525069 nyct-gtfs-1.2.0/nyct_gtfs/compiled_gtfs/
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-12-02 01:56:51.000000 nyct-gtfs-1.2.0/nyct_gtfs/compiled_gtfs/__init__.py
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)    15638 2021-12-02 01:56:51.000000 nyct-gtfs-1.2.0/nyct_gtfs/compiled_gtfs/gtfs_realtime_pb2.py
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)     4671 2021-12-02 01:56:51.000000 nyct-gtfs-1.2.0/nyct_gtfs/compiled_gtfs/nyct_subway_pb2.py
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)     5060 2021-12-09 04:03:53.555340 nyct-gtfs-1.2.0/nyct_gtfs/cpp_parser_wrapper.py
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)    14015 2021-12-09 04:03:57.611311 nyct-gtfs-1.2.0/nyct_gtfs/feed.py
-drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-12-09 04:07:19.532069 nyct-gtfs-1.2.0/nyct_gtfs/gtfs_static/
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)    71961 2021-12-02 01:56:51.000000 nyct-gtfs-1.2.0/nyct_gtfs/gtfs_static/stops.txt
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)  1883488 2021-12-02 01:56:51.000000 nyct-gtfs-1.2.0/nyct_gtfs/gtfs_static/trips.txt
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)     3415 2021-12-02 01:56:51.000000 nyct-gtfs-1.2.0/nyct_gtfs/gtfs_static_types.py
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)     8828 2021-12-02 01:56:51.000000 nyct-gtfs-1.2.0/nyct_gtfs/stop_time_update.py
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)    17492 2021-12-02 01:56:51.000000 nyct-gtfs-1.2.0/nyct_gtfs/trip.py
-drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-12-09 04:07:19.503590 nyct-gtfs-1.2.0/nyct_gtfs.egg-info/
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)    13163 2021-12-09 04:07:19.000000 nyct-gtfs-1.2.0/nyct_gtfs.egg-info/PKG-INFO
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)      533 2021-12-09 04:07:19.000000 nyct-gtfs-1.2.0/nyct_gtfs.egg-info/SOURCES.txt
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)        1 2021-12-09 04:07:19.000000 nyct-gtfs-1.2.0/nyct_gtfs.egg-info/dependency_links.txt
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)       18 2021-12-09 04:07:19.000000 nyct-gtfs-1.2.0/nyct_gtfs.egg-info/requires.txt
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)       10 2021-12-09 04:07:19.000000 nyct-gtfs-1.2.0/nyct_gtfs.egg-info/top_level.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)       38 2021-12-09 04:07:19.547069 nyct-gtfs-1.2.0/setup.cfg
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)      987 2021-12-09 04:01:34.599374 nyct-gtfs-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:43:12.440722 nyct-gtfs-1.3.0/
+-rw-rw-rw-   0        0        0     1094 2021-12-02 01:56:51.000000 nyct-gtfs-1.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0    13488 2023-08-05 18:43:12.439720 nyct-gtfs-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13011 2021-12-02 01:56:51.000000 nyct-gtfs-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 18:43:12.405719 nyct-gtfs-1.3.0/nyct_gtfs/
+-rw-rw-rw-   0        0        0      185 2021-12-02 01:56:51.000000 nyct-gtfs-1.3.0/nyct_gtfs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:43:12.431720 nyct-gtfs-1.3.0/nyct_gtfs/compiled_gtfs/
+-rw-rw-rw-   0        0        0        0 2021-12-02 01:56:51.000000 nyct-gtfs-1.3.0/nyct_gtfs/compiled_gtfs/__init__.py
+-rw-rw-rw-   0        0        0    15638 2021-12-02 01:56:51.000000 nyct-gtfs-1.3.0/nyct_gtfs/compiled_gtfs/gtfs_realtime_pb2.py
+-rw-rw-rw-   0        0        0     4671 2021-12-02 01:56:51.000000 nyct-gtfs-1.3.0/nyct_gtfs/compiled_gtfs/nyct_subway_pb2.py
+-rw-rw-rw-   0        0        0     5060 2023-08-05 18:37:50.000000 nyct-gtfs-1.3.0/nyct_gtfs/cpp_parser_wrapper.py
+-rw-rw-rw-   0        0        0    14597 2023-08-05 18:38:26.000000 nyct-gtfs-1.3.0/nyct_gtfs/feed.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:43:12.433720 nyct-gtfs-1.3.0/nyct_gtfs/gtfs_static/
+-rw-rw-rw-   0        0        0    71961 2021-12-02 01:56:51.000000 nyct-gtfs-1.3.0/nyct_gtfs/gtfs_static/stops.txt
+-rw-rw-rw-   0        0        0  1883488 2021-12-02 01:56:51.000000 nyct-gtfs-1.3.0/nyct_gtfs/gtfs_static/trips.txt
+-rw-rw-rw-   0        0        0     3415 2021-12-02 01:56:51.000000 nyct-gtfs-1.3.0/nyct_gtfs/gtfs_static_types.py
+-rw-rw-rw-   0        0        0     8828 2021-12-02 01:56:51.000000 nyct-gtfs-1.3.0/nyct_gtfs/stop_time_update.py
+-rw-rw-rw-   0        0        0    17492 2023-08-05 18:37:50.000000 nyct-gtfs-1.3.0/nyct_gtfs/trip.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:43:12.427717 nyct-gtfs-1.3.0/nyct_gtfs.egg-info/
+-rw-rw-rw-   0        0        0    13488 2023-08-05 18:43:12.000000 nyct-gtfs-1.3.0/nyct_gtfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2023-08-05 18:43:12.000000 nyct-gtfs-1.3.0/nyct_gtfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 18:43:12.000000 nyct-gtfs-1.3.0/nyct_gtfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-08-05 18:43:12.000000 nyct-gtfs-1.3.0/nyct_gtfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-05 18:43:12.000000 nyct-gtfs-1.3.0/nyct_gtfs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 18:43:12.440722 nyct-gtfs-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      998 2023-08-05 18:39:05.000000 nyct-gtfs-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:43:12.438720 nyct-gtfs-1.3.0/tests/
+-rw-rw-rw-   0        0        0    17819 2023-08-05 18:37:50.000000 nyct-gtfs-1.3.0/tests/test_feed_parse.py
+-rw-rw-rw-   0        0        0    17929 2023-08-05 18:37:50.000000 nyct-gtfs-1.3.0/tests/test_feed_parse_cpp.py
```

### Comparing `nyct-gtfs-1.2.0/LICENSE.txt` & `nyct-gtfs-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.2.0/PKG-INFO` & `nyct-gtfs-1.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,346 +1,344 @@
-Metadata-Version: 2.1
-Name: nyct-gtfs
-Version: 1.2.0
-Summary: Real-time NYC subway data parsing for humans
-Home-page: https://github.com/Andrew-Dickinson/nyct-gtfs
-Author: Andrew Dickinson
-Author-email: andrew.dickinson.0216@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-
-# NYCT-GTFS - Real-time NYC subway data parsing for humans
-[![Contributors][contributors-shield]][contributors-url]
-[![Forks][forks-shield]][forks-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
-[![MIT License][license-shield]][license-url]
-
-This python library provides a human-friendly, native python interface
-for dealing with the [NYCT Subway data published by the MTA](https://api.mta.info/). By default,
-this data is provided in a [protobuf-encoded](https://developers.google.com/protocol-buffers/) format called [GTFS-realtime](https://developers.google.com/transit/gtfs-realtime/), which further
-has [NYCT-specific customization](https://web.archive.org/web/20191221213849/http://datamine.mta.info/sites/all/files/pdfs/GTFS-Realtime-NYC-Subway%20version%201%20dated%207%20Sep.pdf). 
-This is quite difficult to parse, and requires a lot of boilerplate to do even very simple queries. 
-
-However, with NYCT-GTFS, you can access and query this data in just a few lines of Python:
-
-```python
->>> from nyct_gtfs import NYCTFeed
-
-# Load the realtime feed from the MTA site
->>> feed = NYCTFeed("1", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
-# Get all 123 trains currently underway to Times Sq-42 St
->>> trains = feed.filter_trips(line_id=["1", "2", "3"], headed_for_stop_id=["127N", "127S"], underway=True)
-
-# Let's look closer at the first train included in the filter above:
->>> str(trains[0])
-'Northbound 1 to Van Cortlandt Park-242 St, departed origin 22:20:00, Currently INCOMING_AT 34 St-Penn Station, last update at 22:34:11'
-
-# We can extract each of these details programatically as well,
-# to get arrival time information for the next station (which in this case is 34th St-Penn Station):
->>> trains[0].stop_time_updates[0].arrival
-datetime.datetime(2021, 11, 26, 22, 34, 51)
-
-# What about the next stop after that? Should be Times Square
->>> trains[0].stop_time_updates[1].stop_name
-'Times Sq-42 St'
-
-# And what time will it get there?
->>> trains[0].stop_time_updates[1].arrival
-datetime.datetime(2021, 11, 26, 22, 36, 21)
-```
-
-See "Usage Examples" below for more examples of the data available.
-
-### Built With
-
-* [Requests](https://docs.python-requests.org/)
-* [Protocol Buffers](https://developers.google.com/protocol-buffers/)
-* [MTA GTFS-realtime Data Feeds](https://api.mta.info/)
-
-## Installation
-
-1. Get a free MTA API Key at [https://api.mta.info/](https://api.mta.info/#/signup)
-2. Install nyct-gtfs
-   ```sh
-   pip install nyct-gtfs
-   ```
-3. Load the data feed
-    ```python
-    from nyct_gtfs import NYCTFeed
-    
-    # Load the realtime feed from the MTA site
-    feed = NYCTFeed("1", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-    ```
-
-## Usage Examples
-
-### Get All Trip Data from the Feed
-```python
->>> from nyct_gtfs import NYCTFeed
->>> feed = NYCTFeed("B", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
-# Read all trip (train) information published to the BDFM feed 
->>> trains = feed.trips
-
->>> len(trains)
-70
-```
-
-### Filter Only Certain Trip Data from the Feed
-```python
->>> from nyct_gtfs import NYCTFeed
->>> feed = NYCTFeed("B", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
-# Read only D train information from the BDFM feed 
->>> trains = feed.filter_trips(line_id="D")
->>> len(trains)
-26
-
-# Read only D and M train information from the BDFM feed
->>> trains = feed.filter_trips(line_id=["D", "M"])
->>> len(trains)
-43
-
-# TODO
-```
-
-See `NYCTFeed.filter_trips()` for a complete listing of the filtering options available. 
-
-
-### Read Trip/Train Metadata
-```python
->>> from nyct_gtfs import NYCTFeed
->>> feed = NYCTFeed("N", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
-# Read the first train from the feed
->>> train = feed.trips[0]
-
-# Get human-readable summary of the train's status
->>> str(train)
-"Southbound N to Coney Island-Stillwell Av, departed origin 15:12:00, Currently STOPPED_AT 20 Av, last update at 16:22:14"
-
-# Get each piece of this information separately:
->>> train.direction
-"S"
-
->>> train.route_id
-"N"
-
->>> train.headsign_text
-"Coney Island-Stillwell Av"
-
->>> train.departure_time
-datetime.datetime(2021, 11, 27, 15, 21, 00)
-
->>> train.location
-"N06S" # This is the stop ID corresponding to the southbound platform at 20 Av
-
->>> train.location_status
-"STOPPED_AT"
-
->>> train.last_position_update
-datetime.datetime(2021, 11, 27, 16, 22, 14)
-```
-
-See `Trip` for a full list of train metadata fields.
-
-### Read Remaining Stops
-Each trip in the feed has a complete listing of all of its remaining stops. Stops are removed from this listing upon 
-departure from the station listed. Therefore our southbound N train from the previous example still has 20 Av listed 
-in its scheduled stops list:
-```python
->>> from nyct_gtfs import NYCTFeed
->>> feed = NYCTFeed("N", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
-# Read the first train from the feed
->>> train = feed.trips[0]
->>> str(train)
-"Southbound N to Coney Island-Stillwell Av, departed origin 15:12:00, Currently STOPPED_AT 20 Av, last update at 16:22:14"
-
->>> train.stop_time_updates[0].stop_name
-"20 Av"
-
-# We can identify the number of stops this train has left using len()
->>> len(train.stop_time_updates)
-6
-
-# We can also identify the last scheduled stop for this train using a negative list index
->>> train.stop_time_updates[-1].stop_name
-"Coney Island-Stillwell Av"
-```
-
-#### Read stop details
-```python
->>> from nyct_gtfs import NYCTFeed
->>> feed = NYCTFeed("N", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
-# Read the first train from the feed
->>> train = feed.trips[0]
->>> str(train)
-"Southbound N to Coney Island-Stillwell Av, departed origin 15:12:00, Currently STOPPED_AT 20 Av, last update at 16:22:14"
-
->>> train.stop_time_updates[4].stop_name
-"86 St"
-
->>> train.stop_time_updates[4].stop_id
-"N10S"
-
-# Get the estimated arrival time at this stop
->>> train.stop_time_updates[4].arrival
-datetime.datetime(2021, 11, 27, 16, 31, 31)
-```
-
-For full details about stop time fields see `StopTimeUpdate`
-
-### Read Feed Metadata
-
-```python
->>> from nyct_gtfs import NYCTFeed
->>> feed = NYCTFeed("A", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
-# Get the timestamp the GTFS feed was generated at
->>> feed.last_generated
-datetime.datetime(2021, 11, 26, 22, 33, 15)
-
-# Get the GTFS-realtime specification version this feed was derived from
->>> feed.gtfs_realtime_version
-"1.0"
-
-# Get the version of the NYCT extension of the GTFS-realtime specification that this feed is derived from
-# Full specification is available here:
-# https://web.archive.org/web/20191221213849/http://datamine.mta.info/sites/all/files/pdfs/GTFS-Realtime-NYC-Subway%20version%201%20dated%207%20Sep.pdf
->>> feed.nyct_subway_gtfs_version
-"1.0"
-
-# Identify the trip replacement period at the time of generation for this feed
-# This is the period in time that this feed covers (i.e. it "replaces" the prior published schedule for all trips 
-# between the feed generation time and the time listed here). The length of this period can vary by line, but currently
-# it is 30 minutes for all subway lines
->>> feed.trip_replacement_periods
-{
-   'A': datetime.datetime(2021, 11, 26, 23, 03, 15), 
-   'C': datetime.datetime(2021, 11, 26, 23, 03, 15), 
-   'E': datetime.datetime(2021, 11, 26, 23, 03, 15),
-   'H': datetime.datetime(2021, 11, 26, 23, 03, 15),
-   'FS': datetime.datetime(2021, 11, 26, 23, 03, 15)
-}
-
-# Trip replacement periods is also useful to get a list of which subway lines are contained within this feed
->>> feed.trip_replacement_periods.keys()
-dict_keys(['A', 'C', 'E', 'H', 'FS'])
-```
-
-### Refresh Feed Data
-```python
->>> from nyct_gtfs import NYCTFeed
->>> feed = NYCTFeed("A", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
-# Pick a train to get details from
->>> train = feed.trips[0]
->>> train.direction
-"N"
-
-# To pull new data, use the refresh() method
->>> feed.refresh()
-
-# You must also update references to the trains list, existing objects are not modified by refresh()
->>> train = feed.trips[0]
-
-# Note that feed.trips does not necessarily have a stable index across refresh() calls, i.e it is 
-# possible for feed.trips[0] to have changed to represent a different train as a result of the refresh() operation:
->>> train.direction
-"S"
-```
-
-## Feed Groupings
-
-NYCT Subway feeds are grouped by color for all of the B division (lettered) lines. All A division lines
-are grouped into a single feed. When you initialize an `NYCTFeed` object, you can specify a line or feed URL, e.g:
-```python
->>> from nyct_gtfs import NYCTFeed
->>> feed1 = NYCTFeed("A", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
->>> feed2 = NYCTFeed("C", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
->>> feed3 = NYCTFeed("https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-ace", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
->>> feed1.trip_replacement_periods.keys()
-dict_keys(['A', 'C', 'E', 'H', 'FS'])
-
->>> feed2.trip_replacement_periods.keys()
-dict_keys(['A', 'C', 'E', 'H', 'FS'])
-
->>> feed3.trip_replacement_periods.keys()
-dict_keys(['A', 'C', 'E', 'H', 'FS'])
-```
-
-In this example, `feed1`, `feed2`, and `feed3` all pull from the same source, the ACE feed. Provided an update isn't
-published between any of the calls above, they will all contain exactly the same data. Here is a table of the groupings
-as of November 2021. An up-to-date listing can be found [here](https://api.mta.info/#/subwayRealTimeFeeds) (login required).
-
-| Trains        | Feed URL |
-|---------------|-------|
-|  A C E <br/> H ([Rockaway Park Shuttle](https://en.wikipedia.org/wiki/Rockaway_Park_Shuttle)) <br/> FS ([Franklin Av Shuttle](https://en.wikipedia.org/wiki/Franklin_Avenue_Shuttle)) | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-ace |
-| B D F M | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-bdfm |
-| G | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-g |
-| J Z | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-jz |
-| N Q R W | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-nqrw |
-| L |  https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-l |
-| 1 2 3 4 5 6 7 S | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs |
-| SIR ([Staten Island Railway](https://en.wikipedia.org/wiki/Staten_Island_Railway)) | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-si |
-
-
-## Contributing
-
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
-
-If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
-Don't forget to give the project a star! Thanks again!
-
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
-
-## License
-
-Distributed under the MIT License. See `LICENSE.txt` for more information.
-
-## Contact
-
-Andrew Dickinson - andrew.dickinson.0216@gmail.com
-
-Project Link: [https://github.com/Andrew-Dickinson/nyct-gtfs](https://github.com/Andrew-Dickinson/nyct-gtfs)
-
-## Acknowledgments
-
-* [Choose an Open Source License](https://choosealicense.com)
-* [MTA Developer Resources](http://web.mta.info/developers/)
-* [MTA Developer Google Group](https://groups.google.com/g/mtadeveloperresources)
-
-## Disclaimer
-This project is not endorsed by, directly affiliated with, maintained, authorized, or sponsored by any transit agency. 
-All names and marks are the registered trademarks of their original owners. The use of any trade name or trademark is 
-for identification and reference purposes only and does not imply any association with the trademark holder or their 
-brand.
-
-
-[contributors-shield]: https://img.shields.io/github/contributors/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
-[contributors-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/graphs/contributors
-[forks-shield]: https://img.shields.io/github/forks/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
-[forks-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/network/members
-[stars-shield]: https://img.shields.io/github/stars/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
-[stars-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/stargazers
-[issues-shield]: https://img.shields.io/github/issues/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
-[issues-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/issues
-[license-shield]: https://img.shields.io/github/license/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
-[license-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/blob/master/LICENSE.txt
-
+Metadata-Version: 2.1
+Name: nyct-gtfs
+Version: 1.3.0
+Summary: Real-time NYC subway data parsing for humans
+Home-page: https://github.com/Andrew-Dickinson/nyct-gtfs
+Author: Andrew Dickinson
+Author-email: andrew.dickinson.0216@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
+# NYCT-GTFS - Real-time NYC subway data parsing for humans
+[![Contributors][contributors-shield]][contributors-url]
+[![Forks][forks-shield]][forks-url]
+[![Stargazers][stars-shield]][stars-url]
+[![Issues][issues-shield]][issues-url]
+[![MIT License][license-shield]][license-url]
+
+This python library provides a human-friendly, native python interface
+for dealing with the [NYCT Subway data published by the MTA](https://api.mta.info/). By default,
+this data is provided in a [protobuf-encoded](https://developers.google.com/protocol-buffers/) format called [GTFS-realtime](https://developers.google.com/transit/gtfs-realtime/), which further
+has [NYCT-specific customization](https://web.archive.org/web/20191221213849/http://datamine.mta.info/sites/all/files/pdfs/GTFS-Realtime-NYC-Subway%20version%201%20dated%207%20Sep.pdf). 
+This is quite difficult to parse, and requires a lot of boilerplate to do even very simple queries. 
+
+However, with NYCT-GTFS, you can access and query this data in just a few lines of Python:
+
+```python
+>>> from nyct_gtfs import NYCTFeed
+
+# Load the realtime feed from the MTA site
+>>> feed = NYCTFeed("1", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+# Get all 123 trains currently underway to Times Sq-42 St
+>>> trains = feed.filter_trips(line_id=["1", "2", "3"], headed_for_stop_id=["127N", "127S"], underway=True)
+
+# Let's look closer at the first train included in the filter above:
+>>> str(trains[0])
+'Northbound 1 to Van Cortlandt Park-242 St, departed origin 22:20:00, Currently INCOMING_AT 34 St-Penn Station, last update at 22:34:11'
+
+# We can extract each of these details programatically as well,
+# to get arrival time information for the next station (which in this case is 34th St-Penn Station):
+>>> trains[0].stop_time_updates[0].arrival
+datetime.datetime(2021, 11, 26, 22, 34, 51)
+
+# What about the next stop after that? Should be Times Square
+>>> trains[0].stop_time_updates[1].stop_name
+'Times Sq-42 St'
+
+# And what time will it get there?
+>>> trains[0].stop_time_updates[1].arrival
+datetime.datetime(2021, 11, 26, 22, 36, 21)
+```
+
+See "Usage Examples" below for more examples of the data available.
+
+### Built With
+
+* [Requests](https://docs.python-requests.org/)
+* [Protocol Buffers](https://developers.google.com/protocol-buffers/)
+* [MTA GTFS-realtime Data Feeds](https://api.mta.info/)
+
+## Installation
+
+1. Get a free MTA API Key at [https://api.mta.info/](https://api.mta.info/#/signup)
+2. Install nyct-gtfs
+   ```sh
+   pip install nyct-gtfs
+   ```
+3. Load the data feed
+    ```python
+    from nyct_gtfs import NYCTFeed
+    
+    # Load the realtime feed from the MTA site
+    feed = NYCTFeed("1", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+    ```
+
+## Usage Examples
+
+### Get All Trip Data from the Feed
+```python
+>>> from nyct_gtfs import NYCTFeed
+>>> feed = NYCTFeed("B", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+# Read all trip (train) information published to the BDFM feed 
+>>> trains = feed.trips
+
+>>> len(trains)
+70
+```
+
+### Filter Only Certain Trip Data from the Feed
+```python
+>>> from nyct_gtfs import NYCTFeed
+>>> feed = NYCTFeed("B", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+# Read only D train information from the BDFM feed 
+>>> trains = feed.filter_trips(line_id="D")
+>>> len(trains)
+26
+
+# Read only D and M train information from the BDFM feed
+>>> trains = feed.filter_trips(line_id=["D", "M"])
+>>> len(trains)
+43
+
+# TODO
+```
+
+See `NYCTFeed.filter_trips()` for a complete listing of the filtering options available. 
+
+
+### Read Trip/Train Metadata
+```python
+>>> from nyct_gtfs import NYCTFeed
+>>> feed = NYCTFeed("N", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+# Read the first train from the feed
+>>> train = feed.trips[0]
+
+# Get human-readable summary of the train's status
+>>> str(train)
+"Southbound N to Coney Island-Stillwell Av, departed origin 15:12:00, Currently STOPPED_AT 20 Av, last update at 16:22:14"
+
+# Get each piece of this information separately:
+>>> train.direction
+"S"
+
+>>> train.route_id
+"N"
+
+>>> train.headsign_text
+"Coney Island-Stillwell Av"
+
+>>> train.departure_time
+datetime.datetime(2021, 11, 27, 15, 21, 00)
+
+>>> train.location
+"N06S" # This is the stop ID corresponding to the southbound platform at 20 Av
+
+>>> train.location_status
+"STOPPED_AT"
+
+>>> train.last_position_update
+datetime.datetime(2021, 11, 27, 16, 22, 14)
+```
+
+See `Trip` for a full list of train metadata fields.
+
+### Read Remaining Stops
+Each trip in the feed has a complete listing of all of its remaining stops. Stops are removed from this listing upon 
+departure from the station listed. Therefore our southbound N train from the previous example still has 20 Av listed 
+in its scheduled stops list:
+```python
+>>> from nyct_gtfs import NYCTFeed
+>>> feed = NYCTFeed("N", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+# Read the first train from the feed
+>>> train = feed.trips[0]
+>>> str(train)
+"Southbound N to Coney Island-Stillwell Av, departed origin 15:12:00, Currently STOPPED_AT 20 Av, last update at 16:22:14"
+
+>>> train.stop_time_updates[0].stop_name
+"20 Av"
+
+# We can identify the number of stops this train has left using len()
+>>> len(train.stop_time_updates)
+6
+
+# We can also identify the last scheduled stop for this train using a negative list index
+>>> train.stop_time_updates[-1].stop_name
+"Coney Island-Stillwell Av"
+```
+
+#### Read stop details
+```python
+>>> from nyct_gtfs import NYCTFeed
+>>> feed = NYCTFeed("N", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+# Read the first train from the feed
+>>> train = feed.trips[0]
+>>> str(train)
+"Southbound N to Coney Island-Stillwell Av, departed origin 15:12:00, Currently STOPPED_AT 20 Av, last update at 16:22:14"
+
+>>> train.stop_time_updates[4].stop_name
+"86 St"
+
+>>> train.stop_time_updates[4].stop_id
+"N10S"
+
+# Get the estimated arrival time at this stop
+>>> train.stop_time_updates[4].arrival
+datetime.datetime(2021, 11, 27, 16, 31, 31)
+```
+
+For full details about stop time fields see `StopTimeUpdate`
+
+### Read Feed Metadata
+
+```python
+>>> from nyct_gtfs import NYCTFeed
+>>> feed = NYCTFeed("A", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+# Get the timestamp the GTFS feed was generated at
+>>> feed.last_generated
+datetime.datetime(2021, 11, 26, 22, 33, 15)
+
+# Get the GTFS-realtime specification version this feed was derived from
+>>> feed.gtfs_realtime_version
+"1.0"
+
+# Get the version of the NYCT extension of the GTFS-realtime specification that this feed is derived from
+# Full specification is available here:
+# https://web.archive.org/web/20191221213849/http://datamine.mta.info/sites/all/files/pdfs/GTFS-Realtime-NYC-Subway%20version%201%20dated%207%20Sep.pdf
+>>> feed.nyct_subway_gtfs_version
+"1.0"
+
+# Identify the trip replacement period at the time of generation for this feed
+# This is the period in time that this feed covers (i.e. it "replaces" the prior published schedule for all trips 
+# between the feed generation time and the time listed here). The length of this period can vary by line, but currently
+# it is 30 minutes for all subway lines
+>>> feed.trip_replacement_periods
+{
+   'A': datetime.datetime(2021, 11, 26, 23, 03, 15), 
+   'C': datetime.datetime(2021, 11, 26, 23, 03, 15), 
+   'E': datetime.datetime(2021, 11, 26, 23, 03, 15),
+   'H': datetime.datetime(2021, 11, 26, 23, 03, 15),
+   'FS': datetime.datetime(2021, 11, 26, 23, 03, 15)
+}
+
+# Trip replacement periods is also useful to get a list of which subway lines are contained within this feed
+>>> feed.trip_replacement_periods.keys()
+dict_keys(['A', 'C', 'E', 'H', 'FS'])
+```
+
+### Refresh Feed Data
+```python
+>>> from nyct_gtfs import NYCTFeed
+>>> feed = NYCTFeed("A", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+# Pick a train to get details from
+>>> train = feed.trips[0]
+>>> train.direction
+"N"
+
+# To pull new data, use the refresh() method
+>>> feed.refresh()
+
+# You must also update references to the trains list, existing objects are not modified by refresh()
+>>> train = feed.trips[0]
+
+# Note that feed.trips does not necessarily have a stable index across refresh() calls, i.e it is 
+# possible for feed.trips[0] to have changed to represent a different train as a result of the refresh() operation:
+>>> train.direction
+"S"
+```
+
+## Feed Groupings
+
+NYCT Subway feeds are grouped by color for all of the B division (lettered) lines. All A division lines
+are grouped into a single feed. When you initialize an `NYCTFeed` object, you can specify a line or feed URL, e.g:
+```python
+>>> from nyct_gtfs import NYCTFeed
+>>> feed1 = NYCTFeed("A", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+>>> feed2 = NYCTFeed("C", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+>>> feed3 = NYCTFeed("https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-ace", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+>>> feed1.trip_replacement_periods.keys()
+dict_keys(['A', 'C', 'E', 'H', 'FS'])
+
+>>> feed2.trip_replacement_periods.keys()
+dict_keys(['A', 'C', 'E', 'H', 'FS'])
+
+>>> feed3.trip_replacement_periods.keys()
+dict_keys(['A', 'C', 'E', 'H', 'FS'])
+```
+
+In this example, `feed1`, `feed2`, and `feed3` all pull from the same source, the ACE feed. Provided an update isn't
+published between any of the calls above, they will all contain exactly the same data. Here is a table of the groupings
+as of November 2021. An up-to-date listing can be found [here](https://api.mta.info/#/subwayRealTimeFeeds) (login required).
+
+| Trains        | Feed URL |
+|---------------|-------|
+|  A C E <br/> H ([Rockaway Park Shuttle](https://en.wikipedia.org/wiki/Rockaway_Park_Shuttle)) <br/> FS ([Franklin Av Shuttle](https://en.wikipedia.org/wiki/Franklin_Avenue_Shuttle)) | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-ace |
+| B D F M | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-bdfm |
+| G | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-g |
+| J Z | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-jz |
+| N Q R W | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-nqrw |
+| L |  https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-l |
+| 1 2 3 4 5 6 7 S | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs |
+| SIR ([Staten Island Railway](https://en.wikipedia.org/wiki/Staten_Island_Railway)) | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-si |
+
+
+## Contributing
+
+Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+
+If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
+Don't forget to give the project a star! Thanks again!
+
+1. Fork the Project
+2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the Branch (`git push origin feature/AmazingFeature`)
+5. Open a Pull Request
+
+## License
+
+Distributed under the MIT License. See `LICENSE.txt` for more information.
+
+## Contact
+
+Andrew Dickinson - andrew.dickinson.0216@gmail.com
+
+Project Link: [https://github.com/Andrew-Dickinson/nyct-gtfs](https://github.com/Andrew-Dickinson/nyct-gtfs)
+
+## Acknowledgments
+
+* [Choose an Open Source License](https://choosealicense.com)
+* [MTA Developer Resources](http://web.mta.info/developers/)
+* [MTA Developer Google Group](https://groups.google.com/g/mtadeveloperresources)
+
+## Disclaimer
+This project is not endorsed by, directly affiliated with, maintained, authorized, or sponsored by any transit agency. 
+All names and marks are the registered trademarks of their original owners. The use of any trade name or trademark is 
+for identification and reference purposes only and does not imply any association with the trademark holder or their 
+brand.
+
+
+[contributors-shield]: https://img.shields.io/github/contributors/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
+[contributors-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/graphs/contributors
+[forks-shield]: https://img.shields.io/github/forks/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
+[forks-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/network/members
+[stars-shield]: https://img.shields.io/github/stars/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
+[stars-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/stargazers
+[issues-shield]: https://img.shields.io/github/issues/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
+[issues-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/issues
+[license-shield]: https://img.shields.io/github/license/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
+[license-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/blob/master/LICENSE.txt
```

### Comparing `nyct-gtfs-1.2.0/README.md` & `nyct-gtfs-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.2.0/nyct_gtfs/compiled_gtfs/gtfs_realtime_pb2.py` & `nyct-gtfs-1.3.0/nyct_gtfs/compiled_gtfs/gtfs_realtime_pb2.py`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.2.0/nyct_gtfs/compiled_gtfs/nyct_subway_pb2.py` & `nyct-gtfs-1.3.0/nyct_gtfs/compiled_gtfs/nyct_subway_pb2.py`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.2.0/nyct_gtfs/cpp_parser_wrapper.py` & `nyct-gtfs-1.3.0/nyct_gtfs/cpp_parser_wrapper.py`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.2.0/nyct_gtfs/feed.py` & `nyct-gtfs-1.3.0/nyct_gtfs/feed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
 from urllib.parse import urlparse, unquote
 
 import requests
+import httpx
 
 from nyct_gtfs.compiled_gtfs import nyct_subway_pb2, gtfs_realtime_pb2
 from nyct_gtfs.gtfs_static_types import TripShapes, Stations
 from nyct_gtfs.trip import Trip
 
 
 class NYCTFeed:
@@ -121,14 +122,25 @@
         if response.status_code == 403:
             raise RuntimeError(f"Invalid API key: {self._api_key}")
         elif response.status_code != 200:
             raise RuntimeError(f"Error accessing MTA data feed: {response.content}")
 
         self.load_gtfs_bytes(response.content)
 
+    async def refresh_async(self):
+        """Reload this object's feed information from the MTA API async"""
+        async with httpx.AsyncClient() as client:
+            response = await client.get(self._feed_url, headers={'x-api-key':self._api_key})
+            if response.status_code == 403:
+                raise RuntimeError(f"Invalid API key: {self._api_key}")
+            elif response.status_code != 200:
+                raise RuntimeError(f"Error accessing MTA data feed: {response.content}")
+
+            self.load_gtfs_bytes(response.content)
+
     def load_gtfs_bytes(self, gtfs_bytes, cpp_accelerated=False):
         """
         Load this object's feed information from a binary GTFS string, useful for testing or analyzing stored feed data
         """
         if not cpp_accelerated:
             feed = gtfs_realtime_pb2.FeedMessage()
             feed.ParseFromString(gtfs_bytes)
```

### Comparing `nyct-gtfs-1.2.0/nyct_gtfs/gtfs_static/stops.txt` & `nyct-gtfs-1.3.0/nyct_gtfs/gtfs_static/stops.txt`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.2.0/nyct_gtfs/gtfs_static/trips.txt` & `nyct-gtfs-1.3.0/nyct_gtfs/gtfs_static/trips.txt`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.2.0/nyct_gtfs/gtfs_static_types.py` & `nyct-gtfs-1.3.0/nyct_gtfs/gtfs_static_types.py`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.2.0/nyct_gtfs/stop_time_update.py` & `nyct-gtfs-1.3.0/nyct_gtfs/stop_time_update.py`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.2.0/nyct_gtfs/trip.py` & `nyct-gtfs-1.3.0/nyct_gtfs/trip.py`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.2.0/nyct_gtfs.egg-info/PKG-INFO` & `nyct-gtfs-1.3.0/nyct_gtfs.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,346 +1,344 @@
-Metadata-Version: 2.1
-Name: nyct-gtfs
-Version: 1.2.0
-Summary: Real-time NYC subway data parsing for humans
-Home-page: https://github.com/Andrew-Dickinson/nyct-gtfs
-Author: Andrew Dickinson
-Author-email: andrew.dickinson.0216@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-
-# NYCT-GTFS - Real-time NYC subway data parsing for humans
-[![Contributors][contributors-shield]][contributors-url]
-[![Forks][forks-shield]][forks-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
-[![MIT License][license-shield]][license-url]
-
-This python library provides a human-friendly, native python interface
-for dealing with the [NYCT Subway data published by the MTA](https://api.mta.info/). By default,
-this data is provided in a [protobuf-encoded](https://developers.google.com/protocol-buffers/) format called [GTFS-realtime](https://developers.google.com/transit/gtfs-realtime/), which further
-has [NYCT-specific customization](https://web.archive.org/web/20191221213849/http://datamine.mta.info/sites/all/files/pdfs/GTFS-Realtime-NYC-Subway%20version%201%20dated%207%20Sep.pdf). 
-This is quite difficult to parse, and requires a lot of boilerplate to do even very simple queries. 
-
-However, with NYCT-GTFS, you can access and query this data in just a few lines of Python:
-
-```python
->>> from nyct_gtfs import NYCTFeed
-
-# Load the realtime feed from the MTA site
->>> feed = NYCTFeed("1", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
-# Get all 123 trains currently underway to Times Sq-42 St
->>> trains = feed.filter_trips(line_id=["1", "2", "3"], headed_for_stop_id=["127N", "127S"], underway=True)
-
-# Let's look closer at the first train included in the filter above:
->>> str(trains[0])
-'Northbound 1 to Van Cortlandt Park-242 St, departed origin 22:20:00, Currently INCOMING_AT 34 St-Penn Station, last update at 22:34:11'
-
-# We can extract each of these details programatically as well,
-# to get arrival time information for the next station (which in this case is 34th St-Penn Station):
->>> trains[0].stop_time_updates[0].arrival
-datetime.datetime(2021, 11, 26, 22, 34, 51)
-
-# What about the next stop after that? Should be Times Square
->>> trains[0].stop_time_updates[1].stop_name
-'Times Sq-42 St'
-
-# And what time will it get there?
->>> trains[0].stop_time_updates[1].arrival
-datetime.datetime(2021, 11, 26, 22, 36, 21)
-```
-
-See "Usage Examples" below for more examples of the data available.
-
-### Built With
-
-* [Requests](https://docs.python-requests.org/)
-* [Protocol Buffers](https://developers.google.com/protocol-buffers/)
-* [MTA GTFS-realtime Data Feeds](https://api.mta.info/)
-
-## Installation
-
-1. Get a free MTA API Key at [https://api.mta.info/](https://api.mta.info/#/signup)
-2. Install nyct-gtfs
-   ```sh
-   pip install nyct-gtfs
-   ```
-3. Load the data feed
-    ```python
-    from nyct_gtfs import NYCTFeed
-    
-    # Load the realtime feed from the MTA site
-    feed = NYCTFeed("1", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-    ```
-
-## Usage Examples
-
-### Get All Trip Data from the Feed
-```python
->>> from nyct_gtfs import NYCTFeed
->>> feed = NYCTFeed("B", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
-# Read all trip (train) information published to the BDFM feed 
->>> trains = feed.trips
-
->>> len(trains)
-70
-```
-
-### Filter Only Certain Trip Data from the Feed
-```python
->>> from nyct_gtfs import NYCTFeed
->>> feed = NYCTFeed("B", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
-# Read only D train information from the BDFM feed 
->>> trains = feed.filter_trips(line_id="D")
->>> len(trains)
-26
-
-# Read only D and M train information from the BDFM feed
->>> trains = feed.filter_trips(line_id=["D", "M"])
->>> len(trains)
-43
-
-# TODO
-```
-
-See `NYCTFeed.filter_trips()` for a complete listing of the filtering options available. 
-
-
-### Read Trip/Train Metadata
-```python
->>> from nyct_gtfs import NYCTFeed
->>> feed = NYCTFeed("N", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
-# Read the first train from the feed
->>> train = feed.trips[0]
-
-# Get human-readable summary of the train's status
->>> str(train)
-"Southbound N to Coney Island-Stillwell Av, departed origin 15:12:00, Currently STOPPED_AT 20 Av, last update at 16:22:14"
-
-# Get each piece of this information separately:
->>> train.direction
-"S"
-
->>> train.route_id
-"N"
-
->>> train.headsign_text
-"Coney Island-Stillwell Av"
-
->>> train.departure_time
-datetime.datetime(2021, 11, 27, 15, 21, 00)
-
->>> train.location
-"N06S" # This is the stop ID corresponding to the southbound platform at 20 Av
-
->>> train.location_status
-"STOPPED_AT"
-
->>> train.last_position_update
-datetime.datetime(2021, 11, 27, 16, 22, 14)
-```
-
-See `Trip` for a full list of train metadata fields.
-
-### Read Remaining Stops
-Each trip in the feed has a complete listing of all of its remaining stops. Stops are removed from this listing upon 
-departure from the station listed. Therefore our southbound N train from the previous example still has 20 Av listed 
-in its scheduled stops list:
-```python
->>> from nyct_gtfs import NYCTFeed
->>> feed = NYCTFeed("N", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
-# Read the first train from the feed
->>> train = feed.trips[0]
->>> str(train)
-"Southbound N to Coney Island-Stillwell Av, departed origin 15:12:00, Currently STOPPED_AT 20 Av, last update at 16:22:14"
-
->>> train.stop_time_updates[0].stop_name
-"20 Av"
-
-# We can identify the number of stops this train has left using len()
->>> len(train.stop_time_updates)
-6
-
-# We can also identify the last scheduled stop for this train using a negative list index
->>> train.stop_time_updates[-1].stop_name
-"Coney Island-Stillwell Av"
-```
-
-#### Read stop details
-```python
->>> from nyct_gtfs import NYCTFeed
->>> feed = NYCTFeed("N", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
-# Read the first train from the feed
->>> train = feed.trips[0]
->>> str(train)
-"Southbound N to Coney Island-Stillwell Av, departed origin 15:12:00, Currently STOPPED_AT 20 Av, last update at 16:22:14"
-
->>> train.stop_time_updates[4].stop_name
-"86 St"
-
->>> train.stop_time_updates[4].stop_id
-"N10S"
-
-# Get the estimated arrival time at this stop
->>> train.stop_time_updates[4].arrival
-datetime.datetime(2021, 11, 27, 16, 31, 31)
-```
-
-For full details about stop time fields see `StopTimeUpdate`
-
-### Read Feed Metadata
-
-```python
->>> from nyct_gtfs import NYCTFeed
->>> feed = NYCTFeed("A", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
-# Get the timestamp the GTFS feed was generated at
->>> feed.last_generated
-datetime.datetime(2021, 11, 26, 22, 33, 15)
-
-# Get the GTFS-realtime specification version this feed was derived from
->>> feed.gtfs_realtime_version
-"1.0"
-
-# Get the version of the NYCT extension of the GTFS-realtime specification that this feed is derived from
-# Full specification is available here:
-# https://web.archive.org/web/20191221213849/http://datamine.mta.info/sites/all/files/pdfs/GTFS-Realtime-NYC-Subway%20version%201%20dated%207%20Sep.pdf
->>> feed.nyct_subway_gtfs_version
-"1.0"
-
-# Identify the trip replacement period at the time of generation for this feed
-# This is the period in time that this feed covers (i.e. it "replaces" the prior published schedule for all trips 
-# between the feed generation time and the time listed here). The length of this period can vary by line, but currently
-# it is 30 minutes for all subway lines
->>> feed.trip_replacement_periods
-{
-   'A': datetime.datetime(2021, 11, 26, 23, 03, 15), 
-   'C': datetime.datetime(2021, 11, 26, 23, 03, 15), 
-   'E': datetime.datetime(2021, 11, 26, 23, 03, 15),
-   'H': datetime.datetime(2021, 11, 26, 23, 03, 15),
-   'FS': datetime.datetime(2021, 11, 26, 23, 03, 15)
-}
-
-# Trip replacement periods is also useful to get a list of which subway lines are contained within this feed
->>> feed.trip_replacement_periods.keys()
-dict_keys(['A', 'C', 'E', 'H', 'FS'])
-```
-
-### Refresh Feed Data
-```python
->>> from nyct_gtfs import NYCTFeed
->>> feed = NYCTFeed("A", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
-# Pick a train to get details from
->>> train = feed.trips[0]
->>> train.direction
-"N"
-
-# To pull new data, use the refresh() method
->>> feed.refresh()
-
-# You must also update references to the trains list, existing objects are not modified by refresh()
->>> train = feed.trips[0]
-
-# Note that feed.trips does not necessarily have a stable index across refresh() calls, i.e it is 
-# possible for feed.trips[0] to have changed to represent a different train as a result of the refresh() operation:
->>> train.direction
-"S"
-```
-
-## Feed Groupings
-
-NYCT Subway feeds are grouped by color for all of the B division (lettered) lines. All A division lines
-are grouped into a single feed. When you initialize an `NYCTFeed` object, you can specify a line or feed URL, e.g:
-```python
->>> from nyct_gtfs import NYCTFeed
->>> feed1 = NYCTFeed("A", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
->>> feed2 = NYCTFeed("C", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
->>> feed3 = NYCTFeed("https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-ace", api_key="YOUR_MTA_API_KEY_GOES_HERE")
-
->>> feed1.trip_replacement_periods.keys()
-dict_keys(['A', 'C', 'E', 'H', 'FS'])
-
->>> feed2.trip_replacement_periods.keys()
-dict_keys(['A', 'C', 'E', 'H', 'FS'])
-
->>> feed3.trip_replacement_periods.keys()
-dict_keys(['A', 'C', 'E', 'H', 'FS'])
-```
-
-In this example, `feed1`, `feed2`, and `feed3` all pull from the same source, the ACE feed. Provided an update isn't
-published between any of the calls above, they will all contain exactly the same data. Here is a table of the groupings
-as of November 2021. An up-to-date listing can be found [here](https://api.mta.info/#/subwayRealTimeFeeds) (login required).
-
-| Trains        | Feed URL |
-|---------------|-------|
-|  A C E <br/> H ([Rockaway Park Shuttle](https://en.wikipedia.org/wiki/Rockaway_Park_Shuttle)) <br/> FS ([Franklin Av Shuttle](https://en.wikipedia.org/wiki/Franklin_Avenue_Shuttle)) | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-ace |
-| B D F M | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-bdfm |
-| G | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-g |
-| J Z | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-jz |
-| N Q R W | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-nqrw |
-| L |  https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-l |
-| 1 2 3 4 5 6 7 S | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs |
-| SIR ([Staten Island Railway](https://en.wikipedia.org/wiki/Staten_Island_Railway)) | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-si |
-
-
-## Contributing
-
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
-
-If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
-Don't forget to give the project a star! Thanks again!
-
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
-
-## License
-
-Distributed under the MIT License. See `LICENSE.txt` for more information.
-
-## Contact
-
-Andrew Dickinson - andrew.dickinson.0216@gmail.com
-
-Project Link: [https://github.com/Andrew-Dickinson/nyct-gtfs](https://github.com/Andrew-Dickinson/nyct-gtfs)
-
-## Acknowledgments
-
-* [Choose an Open Source License](https://choosealicense.com)
-* [MTA Developer Resources](http://web.mta.info/developers/)
-* [MTA Developer Google Group](https://groups.google.com/g/mtadeveloperresources)
-
-## Disclaimer
-This project is not endorsed by, directly affiliated with, maintained, authorized, or sponsored by any transit agency. 
-All names and marks are the registered trademarks of their original owners. The use of any trade name or trademark is 
-for identification and reference purposes only and does not imply any association with the trademark holder or their 
-brand.
-
-
-[contributors-shield]: https://img.shields.io/github/contributors/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
-[contributors-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/graphs/contributors
-[forks-shield]: https://img.shields.io/github/forks/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
-[forks-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/network/members
-[stars-shield]: https://img.shields.io/github/stars/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
-[stars-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/stargazers
-[issues-shield]: https://img.shields.io/github/issues/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
-[issues-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/issues
-[license-shield]: https://img.shields.io/github/license/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
-[license-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/blob/master/LICENSE.txt
-
+Metadata-Version: 2.1
+Name: nyct-gtfs
+Version: 1.3.0
+Summary: Real-time NYC subway data parsing for humans
+Home-page: https://github.com/Andrew-Dickinson/nyct-gtfs
+Author: Andrew Dickinson
+Author-email: andrew.dickinson.0216@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
+# NYCT-GTFS - Real-time NYC subway data parsing for humans
+[![Contributors][contributors-shield]][contributors-url]
+[![Forks][forks-shield]][forks-url]
+[![Stargazers][stars-shield]][stars-url]
+[![Issues][issues-shield]][issues-url]
+[![MIT License][license-shield]][license-url]
+
+This python library provides a human-friendly, native python interface
+for dealing with the [NYCT Subway data published by the MTA](https://api.mta.info/). By default,
+this data is provided in a [protobuf-encoded](https://developers.google.com/protocol-buffers/) format called [GTFS-realtime](https://developers.google.com/transit/gtfs-realtime/), which further
+has [NYCT-specific customization](https://web.archive.org/web/20191221213849/http://datamine.mta.info/sites/all/files/pdfs/GTFS-Realtime-NYC-Subway%20version%201%20dated%207%20Sep.pdf). 
+This is quite difficult to parse, and requires a lot of boilerplate to do even very simple queries. 
+
+However, with NYCT-GTFS, you can access and query this data in just a few lines of Python:
+
+```python
+>>> from nyct_gtfs import NYCTFeed
+
+# Load the realtime feed from the MTA site
+>>> feed = NYCTFeed("1", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+# Get all 123 trains currently underway to Times Sq-42 St
+>>> trains = feed.filter_trips(line_id=["1", "2", "3"], headed_for_stop_id=["127N", "127S"], underway=True)
+
+# Let's look closer at the first train included in the filter above:
+>>> str(trains[0])
+'Northbound 1 to Van Cortlandt Park-242 St, departed origin 22:20:00, Currently INCOMING_AT 34 St-Penn Station, last update at 22:34:11'
+
+# We can extract each of these details programatically as well,
+# to get arrival time information for the next station (which in this case is 34th St-Penn Station):
+>>> trains[0].stop_time_updates[0].arrival
+datetime.datetime(2021, 11, 26, 22, 34, 51)
+
+# What about the next stop after that? Should be Times Square
+>>> trains[0].stop_time_updates[1].stop_name
+'Times Sq-42 St'
+
+# And what time will it get there?
+>>> trains[0].stop_time_updates[1].arrival
+datetime.datetime(2021, 11, 26, 22, 36, 21)
+```
+
+See "Usage Examples" below for more examples of the data available.
+
+### Built With
+
+* [Requests](https://docs.python-requests.org/)
+* [Protocol Buffers](https://developers.google.com/protocol-buffers/)
+* [MTA GTFS-realtime Data Feeds](https://api.mta.info/)
+
+## Installation
+
+1. Get a free MTA API Key at [https://api.mta.info/](https://api.mta.info/#/signup)
+2. Install nyct-gtfs
+   ```sh
+   pip install nyct-gtfs
+   ```
+3. Load the data feed
+    ```python
+    from nyct_gtfs import NYCTFeed
+    
+    # Load the realtime feed from the MTA site
+    feed = NYCTFeed("1", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+    ```
+
+## Usage Examples
+
+### Get All Trip Data from the Feed
+```python
+>>> from nyct_gtfs import NYCTFeed
+>>> feed = NYCTFeed("B", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+# Read all trip (train) information published to the BDFM feed 
+>>> trains = feed.trips
+
+>>> len(trains)
+70
+```
+
+### Filter Only Certain Trip Data from the Feed
+```python
+>>> from nyct_gtfs import NYCTFeed
+>>> feed = NYCTFeed("B", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+# Read only D train information from the BDFM feed 
+>>> trains = feed.filter_trips(line_id="D")
+>>> len(trains)
+26
+
+# Read only D and M train information from the BDFM feed
+>>> trains = feed.filter_trips(line_id=["D", "M"])
+>>> len(trains)
+43
+
+# TODO
+```
+
+See `NYCTFeed.filter_trips()` for a complete listing of the filtering options available. 
+
+
+### Read Trip/Train Metadata
+```python
+>>> from nyct_gtfs import NYCTFeed
+>>> feed = NYCTFeed("N", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+# Read the first train from the feed
+>>> train = feed.trips[0]
+
+# Get human-readable summary of the train's status
+>>> str(train)
+"Southbound N to Coney Island-Stillwell Av, departed origin 15:12:00, Currently STOPPED_AT 20 Av, last update at 16:22:14"
+
+# Get each piece of this information separately:
+>>> train.direction
+"S"
+
+>>> train.route_id
+"N"
+
+>>> train.headsign_text
+"Coney Island-Stillwell Av"
+
+>>> train.departure_time
+datetime.datetime(2021, 11, 27, 15, 21, 00)
+
+>>> train.location
+"N06S" # This is the stop ID corresponding to the southbound platform at 20 Av
+
+>>> train.location_status
+"STOPPED_AT"
+
+>>> train.last_position_update
+datetime.datetime(2021, 11, 27, 16, 22, 14)
+```
+
+See `Trip` for a full list of train metadata fields.
+
+### Read Remaining Stops
+Each trip in the feed has a complete listing of all of its remaining stops. Stops are removed from this listing upon 
+departure from the station listed. Therefore our southbound N train from the previous example still has 20 Av listed 
+in its scheduled stops list:
+```python
+>>> from nyct_gtfs import NYCTFeed
+>>> feed = NYCTFeed("N", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+# Read the first train from the feed
+>>> train = feed.trips[0]
+>>> str(train)
+"Southbound N to Coney Island-Stillwell Av, departed origin 15:12:00, Currently STOPPED_AT 20 Av, last update at 16:22:14"
+
+>>> train.stop_time_updates[0].stop_name
+"20 Av"
+
+# We can identify the number of stops this train has left using len()
+>>> len(train.stop_time_updates)
+6
+
+# We can also identify the last scheduled stop for this train using a negative list index
+>>> train.stop_time_updates[-1].stop_name
+"Coney Island-Stillwell Av"
+```
+
+#### Read stop details
+```python
+>>> from nyct_gtfs import NYCTFeed
+>>> feed = NYCTFeed("N", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+# Read the first train from the feed
+>>> train = feed.trips[0]
+>>> str(train)
+"Southbound N to Coney Island-Stillwell Av, departed origin 15:12:00, Currently STOPPED_AT 20 Av, last update at 16:22:14"
+
+>>> train.stop_time_updates[4].stop_name
+"86 St"
+
+>>> train.stop_time_updates[4].stop_id
+"N10S"
+
+# Get the estimated arrival time at this stop
+>>> train.stop_time_updates[4].arrival
+datetime.datetime(2021, 11, 27, 16, 31, 31)
+```
+
+For full details about stop time fields see `StopTimeUpdate`
+
+### Read Feed Metadata
+
+```python
+>>> from nyct_gtfs import NYCTFeed
+>>> feed = NYCTFeed("A", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+# Get the timestamp the GTFS feed was generated at
+>>> feed.last_generated
+datetime.datetime(2021, 11, 26, 22, 33, 15)
+
+# Get the GTFS-realtime specification version this feed was derived from
+>>> feed.gtfs_realtime_version
+"1.0"
+
+# Get the version of the NYCT extension of the GTFS-realtime specification that this feed is derived from
+# Full specification is available here:
+# https://web.archive.org/web/20191221213849/http://datamine.mta.info/sites/all/files/pdfs/GTFS-Realtime-NYC-Subway%20version%201%20dated%207%20Sep.pdf
+>>> feed.nyct_subway_gtfs_version
+"1.0"
+
+# Identify the trip replacement period at the time of generation for this feed
+# This is the period in time that this feed covers (i.e. it "replaces" the prior published schedule for all trips 
+# between the feed generation time and the time listed here). The length of this period can vary by line, but currently
+# it is 30 minutes for all subway lines
+>>> feed.trip_replacement_periods
+{
+   'A': datetime.datetime(2021, 11, 26, 23, 03, 15), 
+   'C': datetime.datetime(2021, 11, 26, 23, 03, 15), 
+   'E': datetime.datetime(2021, 11, 26, 23, 03, 15),
+   'H': datetime.datetime(2021, 11, 26, 23, 03, 15),
+   'FS': datetime.datetime(2021, 11, 26, 23, 03, 15)
+}
+
+# Trip replacement periods is also useful to get a list of which subway lines are contained within this feed
+>>> feed.trip_replacement_periods.keys()
+dict_keys(['A', 'C', 'E', 'H', 'FS'])
+```
+
+### Refresh Feed Data
+```python
+>>> from nyct_gtfs import NYCTFeed
+>>> feed = NYCTFeed("A", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+# Pick a train to get details from
+>>> train = feed.trips[0]
+>>> train.direction
+"N"
+
+# To pull new data, use the refresh() method
+>>> feed.refresh()
+
+# You must also update references to the trains list, existing objects are not modified by refresh()
+>>> train = feed.trips[0]
+
+# Note that feed.trips does not necessarily have a stable index across refresh() calls, i.e it is 
+# possible for feed.trips[0] to have changed to represent a different train as a result of the refresh() operation:
+>>> train.direction
+"S"
+```
+
+## Feed Groupings
+
+NYCT Subway feeds are grouped by color for all of the B division (lettered) lines. All A division lines
+are grouped into a single feed. When you initialize an `NYCTFeed` object, you can specify a line or feed URL, e.g:
+```python
+>>> from nyct_gtfs import NYCTFeed
+>>> feed1 = NYCTFeed("A", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+>>> feed2 = NYCTFeed("C", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+>>> feed3 = NYCTFeed("https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-ace", api_key="YOUR_MTA_API_KEY_GOES_HERE")
+
+>>> feed1.trip_replacement_periods.keys()
+dict_keys(['A', 'C', 'E', 'H', 'FS'])
+
+>>> feed2.trip_replacement_periods.keys()
+dict_keys(['A', 'C', 'E', 'H', 'FS'])
+
+>>> feed3.trip_replacement_periods.keys()
+dict_keys(['A', 'C', 'E', 'H', 'FS'])
+```
+
+In this example, `feed1`, `feed2`, and `feed3` all pull from the same source, the ACE feed. Provided an update isn't
+published between any of the calls above, they will all contain exactly the same data. Here is a table of the groupings
+as of November 2021. An up-to-date listing can be found [here](https://api.mta.info/#/subwayRealTimeFeeds) (login required).
+
+| Trains        | Feed URL |
+|---------------|-------|
+|  A C E <br/> H ([Rockaway Park Shuttle](https://en.wikipedia.org/wiki/Rockaway_Park_Shuttle)) <br/> FS ([Franklin Av Shuttle](https://en.wikipedia.org/wiki/Franklin_Avenue_Shuttle)) | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-ace |
+| B D F M | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-bdfm |
+| G | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-g |
+| J Z | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-jz |
+| N Q R W | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-nqrw |
+| L |  https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-l |
+| 1 2 3 4 5 6 7 S | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs |
+| SIR ([Staten Island Railway](https://en.wikipedia.org/wiki/Staten_Island_Railway)) | https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-si |
+
+
+## Contributing
+
+Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+
+If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
+Don't forget to give the project a star! Thanks again!
+
+1. Fork the Project
+2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the Branch (`git push origin feature/AmazingFeature`)
+5. Open a Pull Request
+
+## License
+
+Distributed under the MIT License. See `LICENSE.txt` for more information.
+
+## Contact
+
+Andrew Dickinson - andrew.dickinson.0216@gmail.com
+
+Project Link: [https://github.com/Andrew-Dickinson/nyct-gtfs](https://github.com/Andrew-Dickinson/nyct-gtfs)
+
+## Acknowledgments
+
+* [Choose an Open Source License](https://choosealicense.com)
+* [MTA Developer Resources](http://web.mta.info/developers/)
+* [MTA Developer Google Group](https://groups.google.com/g/mtadeveloperresources)
+
+## Disclaimer
+This project is not endorsed by, directly affiliated with, maintained, authorized, or sponsored by any transit agency. 
+All names and marks are the registered trademarks of their original owners. The use of any trade name or trademark is 
+for identification and reference purposes only and does not imply any association with the trademark holder or their 
+brand.
+
+
+[contributors-shield]: https://img.shields.io/github/contributors/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
+[contributors-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/graphs/contributors
+[forks-shield]: https://img.shields.io/github/forks/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
+[forks-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/network/members
+[stars-shield]: https://img.shields.io/github/stars/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
+[stars-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/stargazers
+[issues-shield]: https://img.shields.io/github/issues/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
+[issues-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/issues
+[license-shield]: https://img.shields.io/github/license/Andrew-Dickinson/nyct-gtfs.svg?style=for-the-badge
+[license-url]: https://github.com/Andrew-Dickinson/nyct-gtfs/blob/master/LICENSE.txt
```

### Comparing `nyct-gtfs-1.2.0/nyct_gtfs.egg-info/SOURCES.txt` & `nyct-gtfs-1.3.0/nyct_gtfs.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -12,8 +12,10 @@
 nyct_gtfs.egg-info/dependency_links.txt
 nyct_gtfs.egg-info/requires.txt
 nyct_gtfs.egg-info/top_level.txt
 nyct_gtfs/compiled_gtfs/__init__.py
 nyct_gtfs/compiled_gtfs/gtfs_realtime_pb2.py
 nyct_gtfs/compiled_gtfs/nyct_subway_pb2.py
 nyct_gtfs/gtfs_static/stops.txt
-nyct_gtfs/gtfs_static/trips.txt
+nyct_gtfs/gtfs_static/trips.txt
+tests/test_feed_parse.py
+tests/test_feed_parse_cpp.py
```

### Comparing `nyct-gtfs-1.2.0/setup.py` & `nyct-gtfs-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="nyct-gtfs",
-    version="1.2.0",
+    version="1.3.0",
     description="Real-time NYC subway data parsing for humans",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Andrew-Dickinson/nyct-gtfs",
     author="Andrew Dickinson",
     author_email="andrew.dickinson.0216@gmail.com",
     license="MIT",
@@ -24,9 +24,9 @@
         "Operating System :: OS Independent"
     ],
     packages=["nyct_gtfs", "nyct_gtfs.compiled_gtfs"],
     include_package_data=True,
     package_data={
         "nyct_gtfs": ["gtfs_static/*.txt"]
     },
-    install_requires=["requests", "protobuf"]
-)
+    install_requires=["requests", "protobuf", "httpx"]
+)
```

