# Annotated Spring: Episode 1 - Spring Boot QuickStart

I want to be able to create Spring Boot projects really easily. I'd like to use Maven as my build tool but I don't want to spend too much time hand crafting a Maven project file. Fortunately the Spring Boot CLI tool helps me accomplish this.

I'm going to be using Java 8 so I have the latest JDK installed already.

    $ java -version

I'm also on a Mac, so I'm going to use Homebrew to install Maven and the Spring Boot CLI. 

First I'll make sure my Homebrew is up to date:

    $ brew update

Then I'll install Maven:

    $ brew install maven

In order to install the Spring Bot CLI I'll need to add a "tap" for their tools to my Homebrew installation. Taps are ???

    $ brew tap pivotal/tap

Now I can install the CLI:

    $ brew install springboot

Let's create a project name 'hello' by using the 'init' command:

    $ spring init hello
    $ cd hello

When we initialized our project it added the Spring Boot Maven plugin to our project which makes it easy to run our app from the command line:

    $ mvn spring-boot:run

Spring Boot also lets us create a self-running JAR, making it easy to distribute our application.

    $ mvn package
    $ java -jar target/demo-0.0.1-SNAPSHOT.jar

## Resources

- [JDK 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
- [Homebrew](http://brew.sh)
- [Maven](https://maven.apache.org)
- [Spring](http://spring.io)
- [Spring Boot](http://projects.spring.io/spring-boot/)
- [Spring Boot CLI](http://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#cli)

