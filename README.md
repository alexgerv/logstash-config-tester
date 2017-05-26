# logstash-config-tester
____

## Description
This small projects allows testing of logstash filters configuration. 



## Configuration
The configuration file is located at `/pipeline/configuration.conf`. It will be reloaded automatically in the logstash instance, no need to restart the containers.

The pipeline flow is:
> input > filters > output 

In this project, the input comes from `stdin` and goes to `stdout`. The only part to touch is the `filters` section. 

## Usage
Simply start this project using `docker-compose run logstash`. 
Then, you only need to paste your log line to see how it is parsed by your filters.