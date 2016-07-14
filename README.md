# jupyterhub-raven-auth

jupyterhub authenticator for the University of Cambridge Raven service.
Written by and for the pyCav Project [2016](http://www.theglobeandmail.com/video/article27108276.ece/ALTERNATES/w620/Video:+Justin+Trudeau+introduces+cabinet+he+says+'looks+like+Canada').


## TODO

### Main
* logout behaviour
* access rights lookup (admins/users)

### Not so main

## Installation

Clone this git repository into a directory.
Install using pip3.

## Configuration

Configure by adding:

> c = get_config()

> c.JupyterHub.authenticator_class = RavenAuthenticator

> c.RavenAuthenticator.description = "pyCav"

