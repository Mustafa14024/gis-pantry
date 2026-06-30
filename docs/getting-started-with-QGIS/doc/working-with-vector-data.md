# Working with Vector Data

[Home](../README.md)


[QGIS Documentation](https://docs.qgis.org/testing/en/docs/gentle_gis_introduction/data_capture.html)


## Index
* Create New Vector Layers
* Select by location
* Create grids and samples
* Joining Data
* [Creating new features](#Creating-new-features)
* [Attribution](#Attribution)
* [Add a field to a layer's attributes](#Add-a-field-to-layer-attributes)
* [Delete Features](#Delete-Features)
* [Moving and adding vertices](#Moving-and-adding-vertices)
* [Snapping](#Snapping)
* [Topological editing](#Topological-editing)
* [Tracing](#tracing)
* [Reshaping](#reshaping)
* [Edit in place](#edit-features-in-place)

  
## Create New Vector Layers
[QGIS Documentation Link](https://docs.qgis.org/testing/en/docs/user_manual/managing_data_source/create_layers.html#id10)

Be sure to check out:  

GIS-Pantry Documentation
* [Scratch and Virtual Layers](Geodatapackage_and_otherformats.md)  

QGIS Documentation  
* [Temporary Scratch layer](https://docs.qgis.org/testing/en/docs/user_manual/managing_data_source/create_layers.html#id15)
* [Virtual layers](https://docs.qgis.org/testing/en/docs/user_manual/managing_data_source/create_layers.html#id22)

## Select by location
Select by location tool isn't found with the other selction tools. You can find select by location in the Vector menu under Research Tools.
![Select By Location](../images/select_by_location.gif "Select By Location")

## Create grids and samples
You can find grid and sample creation tools in the Vector menu under Research Tools.
![Create Grid](../images/create_grid.gif "Create Grid ...")

## Joining Data
[QGIS DOCS](https://docs.qgis.org/testing/en/docs/user_manual/working_with_vector/vector_properties.html#joins-properties)  
QGIS allows joining data by a common field. The join field dialog is accessed through the layer properties under Joins. To add a join from this dialog click the ![Add Join Button](../images/joins_add_button.png "Add New Join Button" ) This will launch the Add Vector Join dialog where you can define your join with the properties:<br>
1.  Join Layer - the layer or table to join to the current layer
2.  Join Field - the join field from the layer or table defined in (1)
3.  Target Field - the field from your source layer to which the attributes from (2) will be joined
4. Toggle to cache the joined table in memory without geometry to speed up attribute lookups
5. Toggle joined field to only join a select number of fields from a table
6. Change the prefix for the joined fields

Additional joins can be added from other layers/tables and joins can be edited with the edit button ![Edit Join Button](../images/joins_edit.png) or removed using the remove button ![Remove Join Button](../images/joins_remove_button.png)

Example of creating a join:<br>
![Creat Join](../images/joins_adding_new.gif "Wowza")

## Creating new features
1. Enable editing on the desired layer
![](../images/Toggle_Editing1.gif)
2. Select the create feature tool and click on the map to start drawing features. When finished, right click to stop drawing
![](../images/Add_Feature.gif)
## Attribution
1. When creating a new feature in a layer with attributes, a pop up will appear asking you to fill in the new feature's attributes
![](../images/Add_Feature_with_Attributes.gif)
2. To edit attributes of an existing feature, open the attribute table, make sure editing is enabled and click into the attribute field to edit the value. (Depending on your settings, you may need to select the features for them to appear in the attribute table)
![](../images/Edit_Attributes.gif)
## Add a field to layer attributes
1. Open the attribute table
2. Make sure editing is enabled
3. Click add field
4. Fill in the field details
![](../images/Add_Field.gif)
## Delete Features
1. In the attributes toolbar, enable the select tool
2. Select the features to be deleted and click the delete features button in the toolbar
![](../images/Delete_Feature.gif)
## Moving and adding vertices  
1. Turn editing on for the desired layer
2. Select the vertex tool from the editing toolbar
## Snapping
1. Add the snapping toolbar by right clicking in the toolbar area and checking the snapping option
2. Click the red magnet ![](../images/snappingMagnet.png) to enable snapping
3. By default, the tolereance is 12 px and snapping is set to vertices only. Change this to vertices and segments if you wish to snap to anywhere on an edge
![](../images/Snapping.gif)
## Topological editing
Topological editing allows you to easily maintain connections between nodes and edges when editing vertices. 
It can be enabled in the snapping toolbar.
![](../images/Topological_Editing.gif)

## Tracing
Tracing allows you to trace your feature against an active layer,all layers, or a custom selection of layers. Tracing also allows you to specify an offset should that be required.
![Trace-o-ramma](../images/editing-tracing.gif)<br>

## Reshaping
Reshaping allows you to change the shape of an selected existing feature. With the desired feature selected and the reshape tool enabled start your reshape change on the same side of the feature you wish to finish. First digitize your reshape line before using right-click to finish.<br>
![Reshape Magic](../images/editing-reshape.gif)

## Edit features in-place
Some prcessing tools can be used to edit features inplace. These processing tools can be run against all features or selected features in a layer with editing toggled on. Some of the tools that support this are: Buffer, Fix Geometries, Force right-hand-rule, Multipart to singleparts, Simplify, Smooth, Clip, Difference, Delete-holes, and others.<br>

![Edit features in-place](../images/editing-inplace.gif)

---
[Back to Top](#Index)
