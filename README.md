# jupyterhub-raven-auth

jupyterhub authenticator for the University of Cambridge Raven service.
Written by and for the pyCav Project (Cavendish Laboratory) [2016](http://www.theglobeandmail.com/video/article27108276.ece/ALTERNATES/w620/Video:+Justin+Trudeau+introduces+cabinet+he+says+'looks+like+Canada').

## Features
* Installs as a plugin, little configuration required
* Customisable login page (with a logo & long description of the service)

## TODO

### Main
* LDAP/College lookup
* Documentation
* General Code Tidying

### Not so main
* access rights lookup (admins/users) (Technically not the purvue of this plugin)

## Installation

Install using pip3.
> pip3 install git+git://github.com/PyCav/jupyterhub-raven-auth.git

## Configuration

Configure by adding:

> c = get_config()

> from raven_auth.raven_auth import RavenAuthenticator

> c.JupyterHub.authenticator_class = RavenAuthenticator

> c.RavenAuthenticator.description = "pyCav"

> c.RavenAuthenticator.long_description = "Welcome to the pyCav Jupyterhub server."

> c.RavenAuthenticator.login_logo = '/absolute/path/to/logo/file'
