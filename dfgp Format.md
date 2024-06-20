# .dfgp Format
- The file format in DFG is named as `.dfgp`, which defines the DFG Storage Model.
- A `.dfgp` file is a ZIP file contains content of a DFG (data frame graph).
- A `.dfgp` file can be thought of as a container that holds a variety of heterogeneous data objects (or datasets). The datasets can be images, tables, graphs, and even documents, such as PDF or Excel.

## Steps to create a .dfgp file
To create a `.dfgp` file you must:
- Add instance files in a dataset to a folder
- Specify an ontology file named `schema.ttl`, which defines the meta information of entities, relations and properties within a dataset.
- Specify a mapping file named `mapping.ttl`, which provides additional mapping information of the defined ontology.
- Compress the folder to a `.dfgp` zip file

## Ontology File Requirements
The requirements of the ontology file in `.dfgp` package are:
1. The file must be named as `schema.ttl`, with a standard RDF Turtle format
2. The file must under the top-level directory
3. Define `rdcn:DataFrameGraph`
4. Define `rdcn:Entity`
5. Define `rdcn:Relation`
6. Define `rdcn:Property`
7. For unstructured properties, the value of `rdfs:range` should be one of the `mediatype` list. Full list on http://skos.semweb.csdb.cn/resource/64d4913c3835f799898237a2

## Mapping File Requirements
The requirements of the mapping file in `.dfgp` package are:
1. The file must be named as `mapping.ttl`, with a standard RDF Turtle format
2. The file must under the top-level directory as the `schema.ttl`
3. Use `rdcn:path` to specify the relative path to the files. It also supports wildcards to match multiple files.








