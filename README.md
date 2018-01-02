### consul
Consul server with web UI

Clone the repo and then build the docker image
	`docker build -t tibco/consul:0.7.5 .`

To launch a standalone Consul server, use:

<!-- -->

	docker run --name consul-agent-node1 -d -p 8500:8500 -p 8400:8400 -p 8600:53/udp -h node1 tibco/consul:0.7.5 -server -bootstrap