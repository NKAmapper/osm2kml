# osm2kml
Convert nodes from OSM to KML file.

### Usage

<code>python osm2kml.py [input filename] [folder tag] [name tag] [description tags]</code>

Parameters:
* _input filename_ - Name of OSM input file.
* _folder tag_ - Tag in OSM file which will be used to group nodes into KML folders (optional; empty value "" permitted).
* _name tag_ - Tag in OSM file which will be used as name tag in KML (default: _name_; empty value "" permitted).
* _description tags_ - List of tags in OSM which will be included in description tag in KML (default: _description_; empty value "" permitted).

The output filename will be the same as the input filename plus ".kml".

### Examples

* <code>python osm2kml.py petrol_stations.osm</code> - No folders, _name_ and _description_ tags from OSM file included by default.
* <code>python osm2kml.py petrol_stations.osm brand branch opening_hours</code> - _Brand_ tag determines folder, _branch_ tag as name, _opening_hours_ as description.
* <code>python osm2kml.py petrol_stations.osm "" branch brand opening_hours</code> - No folders, _branch_ tag as name, _brand_ and _opening_hours_ as description.
