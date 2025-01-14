# MojoHaus BuildPlan Maven Plugin

[![Apache License, Version 2.0, January 2004](https://img.shields.io/github/license/mojohaus/buildplan-maven-plugin.svg?label=License)](http://www.apache.org/licenses/)
[![Maven Central](https://img.shields.io/maven-central/v/org.codehaus.mojo/buildplan-maven-plugin.svg?label=Maven%20Central)](https://search.maven.org/artifact/org.codehaus.mojo/buildplan-maven-plugin)
[![Build Status](https://github.com/mojohaus/buildplan-maven-plugin/actions/workflows/maven.yml/badge.svg)](https://github.com/mojohaus/buildplan-maven-plugin/actions/workflows/maven.yml)
[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/from-referrer/)

A Maven 3.x plugin to inspect the lifecycle of your project. [Documentation](http://www.mojohaus.org/buildplan-maven-plugin/)

### List plugin executions within a project

	mvn buildplan:list

### List plugin executions within phases

	mvn buildplan:list-phase

It is possible to limit the list to a specific phase:

	mvn buildplan:list-phase -Dbuildplan.phase=test

### List plugin executions by plugins

	mvn buildplan:list-plugin

It is possible to limit the list to a specific plugin:

	mvn buildplan:list-plugin -Dbuildplan.plugin=maven-compiler-plugin

### List to output file

	mvn buildplan:list -Dbuildplan.outputFile=buildplan_output.txt

### Report plugin executions within a project

    mvn buildplan:report
