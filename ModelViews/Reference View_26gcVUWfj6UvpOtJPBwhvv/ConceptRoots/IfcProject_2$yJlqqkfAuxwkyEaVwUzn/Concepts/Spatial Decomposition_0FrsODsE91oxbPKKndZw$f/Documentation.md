The _IfcProject_ is used to reference the root of the spatial structure of a building or other construction project (that serves as the primary project breakdown and is required to be hierarchical). The spatial structure elements are linked together, and to the _IfcProject_, by using the objectified relationship _IfcRelAggregates_.

* _IfcProject_.Decomposes -- shall be NIL, i.e. the _IfcProject_ shall be on top of the root of the spatial structure tree.
* _IfcProject_.IsDecomposedBy -- referencing (_IfcSite_ || _IfcBuilding_ || _IfcSpatialZone_) by using _IfcRelAggregates_.RelatedObjects. The _IfcSite_, _IfcBuilding_, or _IfcSpatialZone_ being referenced shall be the root of the spatial structure.