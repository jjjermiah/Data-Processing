# Overview

This is a set of guidelines, tutorials, and standards to follow for pipelines.

Documentation is built using [JetBrains Writerside](https://www.jetbrains.com/help/writerside/)

## Glossary

Pipeline/Workflow
: A set of rules that are run in a specific order to produce a set of output files.

Rule/Step
: A set of commands/scripts that are run to produce a set of output files from a set of input files.

Curator
: The person responsible for maintaining a pipeline and ensuring that it is up-to-date and working correctly.

User
: The person running the pipeline. This could be the same person as the curator, or it could be someone else trying to reproduce the results of the pipeline.

Environment
: The set of software and dependencies that are required to run a pipeline or rule.

Local environment
: The environment on the user's computer. This includes the operating system, software, and dependencies that are installed on the user's computer.

Cluster
: A set of computers that are connected together and used to run jobs in parallel.

Container
: Think of a container as a digital box that holds everything needed to run a program or application. It includes all the necessary files, settings, and tools so that the program can work properly. Containers are isolated from the rest of the system, so they won't interfere with other programs or applications. Learn more at [Docker](https://www.docker.com/resources/what-container).

Repository
: A place where code and other files are stored. This could be a git repository on Github, Gitlab, or Bitbucket, or it could be a folder on a shared drive or cloud storage.

README
: A file that contains information about the repository. This could include instructions on how to run the pipeline, information about the data used in the pipeline, or any other information that is relevant to the pipeline.
