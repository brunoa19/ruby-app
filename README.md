

An image is built in several steps:

0. shipa sets env variables, all envs set with `shipa env-set` are set.
   The build steps from #3 require the following variables to be set:
	    SUPERCRONIC_URL
	    SUPERCRONIC_SHA1SUM
	    SUPERCRONIC

1. shipa installs dependencies from requirements.apt
2. shipa installs ruby version specified in .ruby-version 
3. shipa executes all steps specified in shipa.yaml:hooks:build. 
