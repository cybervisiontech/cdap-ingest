# Cask Data Application Platform (CDAP) Ingest Integration Tests

This project contains set of integration tests for various CDAP ingest project components.
Tests are executed against running CDAP instance. Connection information is configured in properties files.
These files are stored in the resource directory in each sub-module. You can launch the same integration tests with 
different configuration files using maven profiles: it-local, it-local-auth, it-local-auth-ssl, 
it-remote, it-remote-auth and it-remote-auth-ssl.

## Usage

 To launch integration tests against Standalone CDAP instance, execute:
 
 ```
 mvn clean install -P it-local
 ```

 To launch integration tests against Standalone CDAP instance with authentication enabled, execute:
 
 ```
 mvn clean install -P it-local-auth
 ```
 
 To launch integration tests against Standalone CDAP instance with authentication enabled and ssl turned on, execute:
  
  ```
  mvn clean install -P it-local-auth-ssl
  ```
 
 To launch integration tests against Distributed CDAP instance, execute:
 
 ```
 mvn clean install -P it-remote
 ```

 To launch integration tests against Distributed CDAP instance with authentication enabled, execute:
 
 ```
 mvn clean install -P it-remote-auth
 ```
 
 To launch integration tests against Distributed CDAP instance with authentication enabled and ssl turned on, execute:
  
  ```
  mvn clean install -P it-remote-auth-ssl
  ```
 