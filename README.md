###Files naming
Integration tests should be named with IT suffix (example MyTestIT.java, TestIT.groovy):
https://maven.apache.org/surefire/maven-failsafe-plugin/examples/inclusion-exclusion.html

### Integration tests:
mvn clean test -P integration
mvn clean install -P integration

### Default profile dev excludes integration tests:
mvn clean test
mvn clean install
mvn clean test -P dev
mvn clean install -P dev

### Without profiles IT can be skiped with:
mvn clean install -DskipITs