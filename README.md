# Ruby Appdynamics Buildpack
Buildpack that provisions dependencies needed to run AppDynamics, and runs the AppDynamics proxy.

## Usage
Your app's buildpacks execute in a specified order. For example, in a Heroku app's buildpack settings, the buildpack that appears first in the list will execute first, followed by the second, and so on. You should configure Heroku or CloudFoundry so that this buildpack runs before the main one which provisions your application's execution environment, e.g. the Heroku Ruby buildpack.