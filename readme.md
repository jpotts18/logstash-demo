## Logstash demo

### System Dependencies
This tutorial has been done on a Macbook running El Capitan 10.11.6 Make sure that you have a minimum of java 1.7.

`$ java -version`

### Let's bag us an ELK!

`$ brew install elasticsearch logstash kibana`

Let's see what just happened

* `$ brew info elasticsearch`
* `$ brew info logstash`
* `$ brew info kibana`

Let's start up elasticsearch and kibana

* Use brew services if you don't already - `$ brew tap homebrew/services`
* Show the services that are running - `$ brew services list`
* Start up elasticsearch -`$ brew services start elasticsearch`
* Start up kibana - `$ brew services start kibana`

## Demos

1. `$ logstash -f config/01-hello-world/1.conf` learn about stdin and stdout
1. `$ logstash -f config/01-hello-world/2.conf` learn about codec
1. `$ logstash -f config/01-hello-world/3.conf` learn about multiple outputs
1. `$ logstash -f config/01-hello-world/4.conf`
1. `$ logstash -f config/01-hello-world/5.conf`
1. `$ logstash -f config/01-hello-world/6.conf`

1. `$ logstash -f config/02-apache/1.conf`
1. `$ logstash -f config/02-apache/2.conf`

1. `$ logstash -f config/03-twitter/1.conf`
1. `$ logstash -f config/03-twitter/2.conf`
