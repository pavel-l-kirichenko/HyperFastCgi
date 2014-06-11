# HyperFastCgi RoadMap

## version 0.4

### Configuration
* [X] Transports configurations (loglevel)
* [X] AppHost configuration (loglevel, AddTrailingSlash for AspNetHost)
* [ ] Server configuration (select AppHostFactory)

### AppHosts
* [X] Implement general app factory for general application host
* [X] Implement Plain 'Hello, World' 'no System.Web' AppHost
* [X] Implement abstract AppHostBase class with common methods

### AppHostTransport
* [ ] Implement threadpooling/tasks/singlethread support

### GetRoute
* [ ] Implement GetRoute() for managed classes
* [ ] Implement GetRoute() for native classes

### Domain Reloading
* [ ] Implement domain reloading in Server.

### Native Listener
* [ ] Create and start from the new thread (don't block main thread)
* [ ] Implement Shutdown

### Managed Listener
* [X] Remove warnings, check using of stopReceive flag and others

### Refactoring
* [X] Rename namespaces
* [ ] Add 'Core' namespace, move all common things here

### Documentation
* [ ] Document *.config files
* [ ] Document rules of creating custom  

## version 0.5

### OWIN
* [ ] Implement OWIN AppHost

### Unit-testing
* [ ] Create suite, which can select nginx config, server-config, command-line params and run the tests
* [ ] Create WebClient for sending test responses
* [ ] Create AppHosts (aspx, no-web, owin) for testing
* [ ] Create UnitTests ('get' responses, 'post' responses, check headers, check large data, check no data)
* [ ] Add Travis.CI support for tests

### Performance
* [ ] Do performance tests, get the metrics compared to other solutions
* [ ] Improve the results

### Native transports
* [ ] Refactor native bridges: create struct (BridgeClass) which incapsulates .NET  methods 
* [ ] Pass loglevel to native transports and listener
* [ ] Add more logging

### Managed transports
* [ ] Add more logging

## version 0.6

* [ ] AspNet vNext Host implementation