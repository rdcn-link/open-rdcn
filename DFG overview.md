# DFG Overview
The Data Frame Graph (DFG) implements a model for managing and storing data. The model includes an abstract data model and an abstract storage model (the data format), and libraries to implement the abstract model and to map the storage model to different storage mechanisms. The DFG library provides a programming interface to a concrete implementation of the abstract models. The library also implements a model of data transfer, an efficient movement of data from one stored representation to another stored representation. 

The figure below illustrates the relationships between the models and implementations.
<img src=./images/DFG-models-and-implementations.png width=60% />

- **[DFG Abstract Data Model](DFG%20Abstract%20Data%20Model.md)** is a conceptual model of data, data types, and data organization. The abstract data model is independent of storage medium or programming environment.
- **[DFG Storage Model](dfgp%20Format.md)** is a standard representation for the objects of the abstract data model. The `.dfgp` File Format Specification defines the storage model.
- **[The Programming Model]()** is a model of the computing environment and includes platforms from small single systems to large multiprocessors and clusters. The programming model manipulates (instantiates, populates, and retrieves) objects from the abstract data model.
- **[DFG Library](DFG%20Library.md)** is the concrete implementation of the programming model. The library exports the DFG APIs as its interface. In addition to implementing the objects of the abstract data model, the library manages data transfers from one stored form to another. Data transfer examples include reading from disk to memory and writing from memory to disk.
- **[Stored Data]()** is the concrete implementation of the storage model. The Storage Model is mapped to several storage mechanisms including single disk files, multiple files (family of files), and memory representations.
- **[DFG APIs](DFG%20APIs.md)** lists current interfaces provided by the DFG Library.








