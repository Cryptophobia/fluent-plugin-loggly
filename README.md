Loggly plugin for [Fluentd](http://www.fluentd.org)
=============
With fluent-plugin-loggly you will be able to use [Loggly](http://loggly.com) as output the logs you collect with Fluentd.

## Getting Started for Gen2 ([Read here for the difference between Gen1 and Gen2](https://www.loggly.com/docs/gen2-overview-for-gen1-users/))
* Install [Fluentd](http://www.fluentd.org/download)
* gem install fluent-plugin-loggly
* Make sure you have an account with Loggly.
* Configure Fluentd as below:
~~~~~
    <match your_match>
      type loggly
      loggly_url https://logs-01.loggly.com/inputs/xxx-xxxx-xxxx-xxxxx-xxxxxxxxxx
    </match>
~~~~~
    The `xxx-xxxx...` is your Loggly access token.

## Getting Started for Gen 1

* Install fluentd http://fluentd.org
* gem install fluent-plugin-loggly
* Make sure you have an account at loggly.com.
* Create a input.
* Choose service type: HTTP
* JSON logging: true
* Get the url that could by used to do HTTPS POST (this will be used for configuration of the plugin).
  It should be something like https://logs.loggly.com/inputs/xxx-xxxx-xxxx-xxxxx-xxxxxxxxxx


## Parameters
**loggly_url** the url to your loggly input (string).

