# Nmesos 

Nmesos is a tool (CLI tool and sbt plugin) that leverages Singularity 
to deploy new services into Mesos.

## Features

 - Service config in Yaml format.
 - Auto update (scale up instances and resources if needed)
 - [CLI tool](cli/)
 - [Integration with SBT](sbt-plugin/)(optional)
 
# Usage

### Release a service

The following command will read [example-service.yml](sbt-plugin/example-service/example-service.yml)
and try to release the latest tag in the dev environment.

```
nmesos release example-service --environment dev --tag latest
```

# Getting Started with the CLI tool

Install Nmesos cli:

```
brew tap nitro/nmesos  git@github.com:Nitro/nmesos.git
brew install nmesos-cli
```

Update Nmesos cli:
```
brew update
brew upgrade nmesos-cli
```

Uninstall Nmesos cli:
```
brew uninstall nmesos-cli
```

## Usage

./nmesos release example-service --environment dev --tag latest



