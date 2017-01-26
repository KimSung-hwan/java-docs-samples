# Getting Started with Google Stackdriver Monitoring API and the Google Cloud Client libraries

[Google Stackdriver Monitoring API][monitoring] collects metrics, events, and
metadata from Google Cloud Platform, Amazon Web Services (AWS), hosted uptime
probes, application instrumentation, and a variety of common application
components including Cassandra, Nginx, Apache Web Server, Elasticsearch and many
others.

These sample Java applications demonstrate how to access the Stackdriver
Monitoring API using the [Google Cloud Client Library for Java][google-cloud-java].

[monitoring]: https://cloud.google.com/monitoring/docs/
[google-cloud-java]: https://github.com/GoogleCloudPlatform/google-cloud-java

## Quickstart

Install [Maven](http://maven.apache.org/).

Build your project with:

	mvn clean package -DskipTests

You can then run a given `ClassName` via:

	mvn exec:java -Dexec.mainClass=com.example.monitoring.ClassName \
	    -DpropertyName=propertyValue \
		-Dexec.args="arg1 'arg 2' arg3"

### Analyze a string for sentiment (using the quickstart sample)

    mvn exec:java -Dexec.mainClass=com.example.monitoring.QuickstartSample \
        -DprojectId=YOUR_PROJECT_ID