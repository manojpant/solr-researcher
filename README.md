[![Build Status](https://travis-ci.org/sematext/solr-researcher.svg?branch=master)](https://travis-ci.org/sematext/solr-researcher)

# solr-researcher

The Solr ReSearcher project has Solr components that can be used to improve user's search experience.

### Components
Currently, the Solr ReSearcher has two modules, in addition to its core:
* **core** – Common classes for other ReSearcher components
* **relaxer** – Query Relaxer is a Solr component that executes alternative queries when it detects that original query produced poor results or no results at all due to being too restrictive. It transparently returns better search results to the client without the client having to restructure the query and send additional requests to Solr over the wire and re-examine the results.
* **dym** – Solr DYM ReSearcher (aka Did You Mean ReSearcher) is a Solr component that executes alternative queries when it detects that original queries produced poor results or no results at all due to spelling mistakes or typos. It transparently returns better search results to the client.

### Usage
Check usage for each component in their own README.md
* [Solr Query Relaxer](https://github.com/sematext/solr-researcher/tree/master/relaxer)
* [Solr DYM ReSearcher](https://github.com/sematext/solr-researcher/tree/master/dym)


### Solr Version
5.2.X (PRs for newever versions welcome!)

### Maven Artifacts
Maven artifacts are published under https://oss.sonatype.org/content/repositories/snapshots/com/sematext/

To use Solr ReSearcher add the following dependency to your project:

```xml
<dependency>
  <groupId>com.sematext.solr</groupId>
  <artifactId>st-ReSearcher-relaxer</artifactId>
  <version>1.12.5.2.0-SNAPSHOT</version>
</dependency>`
```
or

```xml
<dependency>
  <groupId>com.sematext.solr</groupId>
  <artifactId>st-ReSearcher-dym</artifactId>
  <version>1.12.5.2.0-SNAPSHOT</version>
</dependency>`
```

### Continuous Integration
Continuous Integration environment for Solr ReSearcher project can be found at: https://travis-ci.org/sematext/solr-researcher

### Build

You need maven and JDK 7:

```sh
$ mvn clean package
```

## License
Solr ReSearcher is released under Apache License, Version 2.0

## Contact
* For questions ping [@sematext](http://twitter.com/sematext)
* For support visit http://sematext.com
* Like working with Solr or Elasticsearch?  Please get in touch - we're always looking for good engineers, consultants, trainers, and support engineers.
