# Akka-Kinesis
[Akka .Net](https://github.com/akkadotnet/akka.net/) Library for [AWS Kinesis](https://aws.amazon.com/kinesis)

The project aims to create a libraries to help on scaling consume process for [AWS Kinesis](https://aws.amazon.com/kinesis) streams.

The idea to use [Akka .Net](https://github.com/akkadotnet/akka.net/) project was to create a elastic clustered system capable of process [AWS Kinesis](https://aws.amazon.com/kinesis) stream records without the constrains to have "one consumer per shard" imposed on others libraried. Actor model represent a pretty way to solve this kind of distributed work problem and that's why was choosed to use [Akka .Net](https://github.com/akkadotnet/akka.net/) as framework for this library.

The project focus on created a Actor SubSytem capable of retreive and process stream records but it also has a secondary Subsystem called "Heimdall" that monitore stream stats on [AWS Cloudwatch](https://aws.amazon.com/cloudwatch) and reshard stream always that is needed.

You can read more about the project on [Wiki page](https://github.com/Caldas/Akka-Kinesis/wiki)
