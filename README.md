**FOR DEMONSTRATION PURPOSES ONLY**

# elasticsearch monitoring demo
A demo of elasticsearch monitoring using [metricbeat].

From the docs, it is recommended to have a monitoring cluster separate from the production cluster.

This repository uses Docker to demonstrate this. 

We launch:
- an elasticsearch container for the production cluster
- a metricbeat container to collect elasticsearch metrics (in reality this would be a service installed on the same instance as elasticsearch)
- an elasticsearch container for the monitoring cluster
- a kibana container to view the monitoring data

## Usage
1. Ensure Docker is running
1. Run `./script/start`
1. Open Kibana at `http://localhost:5601/app/monitoring`
1. Run `./script/add-demo-data`
1. Observe monitoring data

<!-- only links below here -->
[metricbeat]: https://www.elastic.co/guide/en/elasticsearch/reference/current/monitoring-production.html
