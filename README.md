*This is an enhancement project as part of the MSR course 2021/22 at UniKo, CS department, SoftLang Team*

*This repositories forks from https://github.com/gorjatschev/applying-apis for MSR 2021/22 Coursework*

# Team
Team: **Mike**
* Jorge Gavilan

# Baseline study

## Research Question
Can we continuously sample projects and aggregate knowledge about combined API usage?

## Input data
CSV files generated after Collection and Selection process:

* output/repositories_with_dependencies.csv 
>[repo_name, [dependencies]]

* output/repositories_selected/[dependenciesString].csv 
> [repo_name]








## Output data
Parsing output files:
* /output/dependencies/dependencies_[reponame].csv  
> [groupId, artifactId, version, mcrCategories, mcrTags, downloaded, dlVersIfDiff,
  jarURL, pathToJAR] 

* /output/data/data_[reponame].csv  
> [filePath, packageName, className, methodName, line, column, javaParserTypeOfElement, usedClassOfElement,
  isAPIClass, api, mcrCategories	mcrTags]



# Implementation

This optmization project uses the code from [Gorjatschev21 repository](https://github.com/gorjatschev/applying-apis) as a baseline. 
Parsing process was intervened in order to generate output files as repositories were parsed, and to modify the order in which
repositories were parsed.


## Hardware requirements
* Operating system: Linux (recommended Ubuntu 16.04 or higher), MacOS, or Windows 7 to 10.
* Memory: At least 4GB RAM (8GB preferable)

## Software requirements
* Java 11
* Java compatible IDE

## Validation
Reported Mixed API Usage (Full parsing Repo set vs Partial parsing)
Execution time  (Full parsing Repo set vs Partial parsing)


# Notes
You need to create a personal access token in your GitHub account and then replace the `USERNAME_AND_TOKEN` in `RepositoriesPicker.java` with your username and token.