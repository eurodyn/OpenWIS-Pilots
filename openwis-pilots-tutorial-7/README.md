## OWT-7: Database communication in Karaf via services
Hibernate ORM (Hibernate in short) is an object-relational mapping tool for the Java programming language. It provides a framework for mapping an object-oriented domain model to a relational database. Hibernate handles object-relational impedance mismatch problems by replacing direct, persistent database accesses with high-level object handling functions.

The purpose of this tutorial is to showcase database communication in an OSGi service. In particular it will:
1. Enhance the service(s) used in OWT-6, and integrate Hibernate into them.
2. Store and read data from an underlying database.