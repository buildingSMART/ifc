The _IfcTessellatedFaceSet_ is a boundary representation topological model limited to planar faces and straight edges. It may represent an approximation of an analytical surface or solid that may be provided in addition to its tessellation as a separate shape representation. The _IfcTessellatedFaceSet_ provides a compact data representation of an connected face set using indices into ordered lists of vertices, normals, colours, and texture maps.

> NOTE&nbsp; The compact representation has been chosen to enable small data sets despite potentially large sets of faces, edges and vertices needed to represent tessellations of analyticals surfaces and solids, and despite large sets of colour and texture information to annotate the tessellated faces.

The _IfcTessellatedFaceSet_ is an abstract supertype of tesselated face sets each imposing specific constraints on face generation for tessellation, such as triangulation (with or without strip and fans), or quadrilaterals.

> NOTE&nbsp; Not all different constraints on face sets are included as specific subtypes in this release of the specification.

The following attributes apply to all subtypes:

* The _Coordinates_ are the ordered list of Cartesian points representing the vertices of the tessellated item. An index list, defined at the level of subtypes, uses the points, identified by index position, to construct the polylines that represent the faces.
* The _Normals_ are the ordered list of directions representing normals of the tessellated item. An index list, defined at the level of subtypes, uses the directions, identified by index position, to define the normals either by face or by edge.
* The _HasColours_ inverse relation provides an indexed colour map with an corresponding list of indices providing a colour for each face of the tessellated face set.
* The _HasTextures_ inverse relation provides an indexed texture map with an corresponding list of indices providing texture coordinates that map to the geometric coordinates of the polylines representing the faces.

Each face of the tessellated face set shall have:

* at least three non-coincident vertices;
* vertices that define a planar polygon;
* vertices that define a non-self-intersecting polygon.

> NOTE&nbsp; The definition of _IfcTessellatedFaceSet_ is based on the **indexedFaceSet** defined in ISO/IEC 19775-1

> HISTORY&nbsp; New entity in IFC4.