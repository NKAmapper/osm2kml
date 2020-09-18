# osm2kml
Convert nodes from OSM to KML file.

### Usage

<code>python osm2kml.py [input_filename] [folder_tag] [name_tag] [description_tags]</code>

Parameters:
* _input_filename_: Name of OSM input file.
* _folder_tag_: Tag in OSM file which will be used to group nodes into KML folders (optional, empty value "" permitted).
* _name_tag_: Tag in OSM file which will be used as name tag in KML (default: _name_, empty value "" permitted).
* _description_tags_: List of tags in OSM which will be included in description tag in KML (default: _description, empty value "" permitted).

The output filename will be the same as the input filename plus ".kml".

### Examples

<code>python osm2kml.py petrol_stations.osm</code>

<code>python osm2kml.py petrol_stations.osm brand branch opening_hours</code>

<code>python osm2kml.py petrol_stations.osm "" branch brand opening_hours</code>
