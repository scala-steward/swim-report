# :swimmer: Swim Report

Simple CLI application that reads a FIT file of a lap swim activity and produces summary statistics.

:warning: **Project is not finished, yet!** :construction: When it is ready, this warning will be removed.

## Features

- Text or JSON output
- General swim activity details
- Total distance swum for each stroke
- Number of pool lengths swum for each stroke
- Longest continuous swim distance for each stroke
- Average swim speed information for each interval
- Average heart rate information
- Total rest time
- Option to force an attempt to read a corrupt FIT file

## Usage

`swim-report` is a CLI application, Java 8 or newer is required to run it.

Read FIT file and display report:

```
java -jar swim-report.jar [--output <text|json>] [--ignore-integrity] <FIT file path>
```

For help on supported options:

```
java -jar swim-report.jar --help
```

## Building from source

JDK 8 or later and [sbt](https://www.scala-sbt.org/) are required to build the application from source.

Use `sbt compile` to compile the sources, `sbt test` to run the tests and `sbt assembly` to build the JAR with all dependencies.
