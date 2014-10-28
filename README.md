[Bridge Closure Map](http://vtrans.maps.arcgis.com/apps/webappviewer/index.html?id=b0d86b0133504e5796357af446bef3ca)
============

_User Story_

"Will a bridge that I travel on be worked on or closed?"

Progress:

- Refine the service by changing the popup header and configuring the fields.
- Share the MXD via GitHub
- Create service [(url)](http://vtransmap01.aot.state.vt.us/arcgis/rest/services/vtp3/BridgeClosures/MapServer)

###Bridge Map Development

1. Used StructuresClosuresPoints Feature Class from GDB_GEN for the Bridge Closure Map.
2. Created Feature Service and added it to new AGO map using "Add Layer from Web" option from Add layer drop-down.
3. Configure Pop-ups by right clicking on the Feature Service in Table of Contents to view Feature Layer.
4. Use Feature Layer drop-down arrow to configure pop-ups.
5. Within pop-up title change default name to Town Name - Route - Bridge No. i.e  (Lowell - VT-100 - Bridge No.1)
6. Click on Configure Attributes highlighted in blue and turn off all layers that were used in Pop-up title to avoid duplication.
7. The only fields that should be on are; Project, Begin Closure, End Closure and Link.
8. Use drop-down arrow to change symbol, then click OPTIONS highlighted in blue to open symbol properties. 
9. Use drop-down arrow within symbol properties to select type of points to choose from. 
10. Used Transportation point type for Yellow Sign with Topo Bridge symbol.
11. Changed Basemap map to OpenStreetMap
12. Added States/Provinces Boundary backgorund layer for popping VT look.
13. Set filter on States/Provinces Boundary to ("postal" is not "VT") and Fill Transperency to 70%.
