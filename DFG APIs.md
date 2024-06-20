# DFG APIs

Current APIs provided by the DFG Libraries:

| Ontology           | API                             | Description                         |
|--------------------|---------------------------------|-------------------------------------|
| DataFrameGraph     | loadDataFrameGraph()            | 输入.dfgp压缩包文件，加载成内存的DataFrameGraph结构 |
|                    | getDfgSchema()                  | 获取DFG的本体描述信息                        |
|                    | listEntities()                  | 列举DFG中全部的Entity本体                   |
|                    | listRelations()                 | 列举DFG中全部的Relation本体                 |
|                    | getEntityByLabel()              | 获取按label筛选的Entity本体                 |
|                    | getRelationByLabel()            | 获取按label筛选的Relation本体               |
|                    | match()                         | 条件查询                                |
| Entity DataFrame   | meta()                          | 获取元信息                               |
|                    | schema()                        | 获取表结构信息                             |
|                    | getProperties()                 | 获取全部属性                              |
|                    | other common APIs for DataFrame | 例如open，limit，select等                |
| Relation DataFrame | meta()                          | 获取元信息                               |
|                    | schema()                        | 获取表结构信息                             |
|                    | getProperties()                 | 获取全部属性                              |
|                    | getFrom(), getTo()              | 获取关联的前后Entity本体                     |
|                    | other common APIs for DataFrame | 例如open，limit，select等                |
