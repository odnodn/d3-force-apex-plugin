# d3-force-apex-plugin

This is mainly a Oracle APEX plugin (but can also used standalone), which uses the [D3 visualization library] (http://d3js.org/) to render a network layout. It has the following features:

  * Interactive customizing wizard
  * Source data can be a XML or JSON string
  * Link directions are visible and self references are rendered in a nice way - have a look in the online demos
  * Node sizes are calculated between given min and max values depending on the "sizevalue" attribute in your source data
  * Node colors are assigned depending on the given "colorvalue" attribute in your source data
  * Optional tooltips depending on the given "infostring" attribute in your source data
  * Nodes can be pinned and the current positions can be saved and loaded to predefine a layout
  * There is a JavaScript API to interact with the graph, also including five events for the nodes (click, dblclick, contextmenu, mouseenter, mouseleave)
  * All five events are available in APEX - the plugin region can be AJAX refreshed and triggers then also apexbeforerefresh and apexafterrefresh

## Links

  * Download of the [latest version] (https://github.com/ogobrecht/d3-force-apex-plugin/releases/latest)
  * Plugin demo on [apex.oracle.com] (https://apex.oracle.com/pls/apex/f?p=18290)
  * Standalone demo on [github.io] (http://ogobrecht.github.io/d3-force-apex-plugin/)
  * Documentation in the [wiki] (https://github.com/ogobrecht/d3-force-apex-plugin/wiki)

## Credits

I would like to say THANK YOU to all the people who share their knowledge. Without this sharing I would not have been able
to create this D3 implementation. Special thanks to Mike Bostock for his great library and to Carsten Czarski for mentoring
me on Oracle APEX plugin development.

## Changelog

### 1.0.3 (2015-01-30)

* Fixed: Configuration - Boolean values are not correct initialized
* Fixed: APEX - Page items to submit not working on AJAX refresh