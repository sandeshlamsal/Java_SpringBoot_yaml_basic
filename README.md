# YAMLinSpringBoot

YAML is a superset of JSON, and as such is a very convenient format for specifying hierarchical 
configuration data. The SpringApplication class will automatically support YAML as an 
alternative to properties whenever you have the SnakeYAML library on your classpath.


Spring Framework provides two convenient classes that can be used to load YAML documents. The YamlPropertiesFactoryBean will load YAML as Properties and the YamlMapFactoryBean will load YAML as a Map.

For example, the following YAML document:

environments:
    dev:
        url: http://dev.bar.com
        name: Developer Setup
    prod:
        url: http://foo.bar.com
        name: My Cool App
Would be transformed into these properties:

environments.dev.url=http://dev.bar.com
environments.dev.name=Developer Setup
environments.prod.url=http://foo.bar.com
environments.prod.name=My Cool App


Reference:http://docs.spring.io/spring-boot/docs/current/reference/html/boot-features-external-config.html#boot-features-external-config-profile-specific-properties
