# jobe
A Dockerised Jobe Server

# Run

To run a new docker container containing the Jobe server type the following:

`docker run -d -p 4000:80 --name jobe jeanpetric/jobe:1.5.0`

# Test

To start with, make sure the server can be accessed and it lists all languages it supports:

`http://<host_running_docker>:4000/jobe/index.php/restapi/languages`

You should get something down the line:

`[["c","7.3.0"],["cpp","7.3.0"],["java","10.0.2"],["nodejs","8.10.0"],["octave","4.2.2"],["pascal","3.0.4"],["php","7.2.7"],["python3","3.6.5"]]`

These are the default languages installed with Jobe server. If you want a specific one fire a request.

# NB

This is a very basic installation of Jobe server - just to get you going (i.e. no firewall is setup)!

For that, you will need to dig into the manual which explains how to set the details up: https://github.com/trampgeek/jobe
