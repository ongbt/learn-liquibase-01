# Liquibase

Ref: 
- https://github.com/liquibase/liquibase-gradle-plugin#usage
- https://www.baeldung.com/liquibase-refactor-schema-of-java-app 
- (some sample codes not correct)
- for reading:
  - https://github.com/thombergs/code-examples/tree/master/spring-boot/data-migration/liquibase
  - https://reflectoring.io/database-migration-spring-boot-liquibase/
  

## Steps:
1. Install liquibase gradle plugin
2. Change build.gradle to include many liquibaseRuntime dependencies
3. Specify the changelog path correctly in build.gradle
4. Run './gradlew build' then `./gradlew update`

## Issues:
1. Rollback doesnt work, need to try again: `gradle rollbackCount -PliquibaseCommandValue=0`
