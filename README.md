# Terrapyn 

#### _Content, Collaboration, and Analytics for Geography._
[See user, administrator, and developer documentation in the wiki](https://github.com/JeffHeard/geoanalytics/wiki)

## About Terrapyn

Terrapyn is an Open Source spatial data and analytics infrastructure based
around unifying many of the open source python geography projects into a
content management and collaboration framework. Terrapyn is meant to be a
framework that handles both classical and exotic formats in a unified way,
setting up a system of drivers that connect these data sources to web services.

From there, data can be catalogued, described, queried, and Terrapyn' CMS
can serve as a host to a myriad of domain-specific applications. 

Terrapyn was developed at [RENCI](http://www.renci.org) to deal with
various projects centered around providing application infrastructure around
scientific geographic data.  It has been used in 11 projects at RENCI in:

* Environemtnal sciences (hydrology, weather modeling)
* Earth science
* Epidemiology
* Public health
* Decision support
* Emergency management and mitigation
* Digital humanities
* Digital media

It is now an integral part of [TerraHub](http://www.terrahub.io), and is used
to provide map tiles and styling to enhance TerraHub's geographic offering. 
TerraHub LLC now commercially supports the Terrapyn project and actively 
contributes to its continued development in Open Source.

## Contribute!

We are actively seeking collaborators and contributors that can help grow the 
usage and sustainability of the Terrapyn endeavor.  The biggest thing we
need right now is documentation.  If you can read Python code and write 
readable documentation either as developer or user documentation, we need your
skills!

## Terrapyn purpose

Geography used to be the exclusive domain of GIS systems such as ArcGIS and
MapInfo.  Web-mapping, data APIs such as those provided by Facebook, Twitter,
and the like, and huge datasets like those that come from NASA have become far
more important to the average researcher and are difficult to work with in
these traditional platforms.  

Terrapyn' lofty goal is to solve this problem and provide a mechanism for
analytists, experts, and researchers to use these data in a way that's
fundamentally easier and more fluid than current tools provide. 

We also aim to provide a way to publish map data in a way that treats 
maps, cartography, and visualization as "not special." We aim for publishing
tools that are more like Wordpress than they are like Apache Server. 

## Terrapyn structure

Terrapyn is based around treating data sources as curated content, and 
on supporting the development of applications and data APIs that enable people
to work with data through a unified, well-understood interface.  Toward this,
we embrace OGC standards for interoperability and will work actively to support
and more fully implement these standards.

We also follow and embrace open source projects in geography and cartography 
that have gained community traction and where these are more widely used or 
more capable than current OGC standards, we adopt these instead.  For example,
rendering maps is provided by [Mapnik](https://www.github.com/mapnik/mapnik)
and stylesheets are compiled through [Carto](http://www.mapbox.com/carto). 

Terrapyn is deployed as a Django project (not an app - see
[Mezzanine](http://mezzanine.jupo.org)'s explanation as to why), incorporating
a number of reusable apps that work in concert:

* terrapyn.geocms: Data publishing, semantics, and metadata.  WMS and soon to be
  WFS web services that provide OGC standard ways of accessing and visualizing
  datasets on a map or providing them to be consumed GIS or analytics systems
  like Arc, SAS, or qGIS.
* terrapyn.ows : WMS and WFS webservice code that can be adapted to projects.
* django_docker_processes : Container driven analytics.  Deploy complex analytics
  as a simple web service that integrates with Terrapyn data using GitHub and Docker!

## Licensing

Terrapyn is licensed under an MIT-style license.  See LICENSE.txt for 
details
