---
layout: doc_page
---

Peons
-----

### Configuration

For Peon Configuration, see [Peon Query Configuration](../configuration/index.html#peon-query-configuration) and [Additional Peon Configuration](../configuration/index.html#additional-peon-configuration).

### HTTP Endpoints

For a list of API endpoints supported by the Peon, please see the [Peon API reference](../operations/api-reference.html#peon).

Peons run a single task in a single JVM. MiddleManager is responsible for creating Peons for running tasks.
Peons should rarely (if ever for testing purposes) be run on their own.

### Running

The peon should very rarely ever be run independent of the middle manager unless for development purposes.

```
org.apache.druid.cli.Main internal peon <task_file> <status_file>
```

The task file contains the task JSON object.
The status file indicates where the task status will be output.

