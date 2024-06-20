# DFG Library
The DFG library is the concrete implementation of the programming model. The DFG Library is linked to an application program which may be written in Java, Scala or Python. The application program implements problem specific algorithms and data structures and calls the DFG library to store and retrieve data. It may also link to other software or services (for example, parsers and transformers for format parsing and transforming).

It is also important to realize that each module manages data using data structures that are appropriate to its layer.

The figure below shows the dependencies of these modules, and data structures used in different layers.
<img src=./images/dfg-library.png width=60% />

- **The Application Program** uses data structures that represent the problem and algorithms including variables, tables and arrays among other data structures. Depending on its design and function, an application may have quite a few different kinds of data structures and different numbers and sizes of objects.
- **The DFG Library** implements the objects of the DFG abstract data model. Some of these objects include Dataset, DataFrame, and MetaData. The application program maps the application data structures to a hierarchy of DFG objects. Each application will create a mapping best suited to its purposes.
- **Storage System** contains the .dfgp format file mapped to the objects of the DFG abstract data model.
- **in-memory storage** uses arrow format to map the objects of the DFG abstract data model.
