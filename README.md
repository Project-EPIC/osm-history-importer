Osm History Importer
=====================
A program for importing OSM History data into a PostGIS database.


Steps:
1. Read an OSM history file (my_area.osh.pbf) with the Libosmium framework from Python with the PyOsmium adapter
2. Import into a PostGIS Database
3. Read unique changesets & users and call the appropriate APIs to import their data.




### Schema Demands
1. Be PostGIS extensible
2. Needs to handle multipel versions of objects (unique on id+version)
3. Needs to handle open tagging scheme (look into JSON columns)
