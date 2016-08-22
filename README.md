# jupyterhub-raven-auth

jupyterhub authenticator for the University of Cambridge Raven service.
Written by and for the pyCav Project (Cavendish Laboratory) [2016](http://www.theglobeandmail.com/video/article27108276.ece/ALTERNATES/w620/Video:+Justin+Trudeau+introduces+cabinet+he+says+'looks+like+Canada').

## Features
* Installs as a plugin, little configuration required
* Whitelisting using the Lookup service (e.g. Department of Physics, or by College)
* Customisable login page (with a logo & long description of the service)

## TODO

### Main
* Test JupyterHub default whitelisting with the Cambridge lookup whitelist
* Documentation

## Installation

Install using pip3.
> pip3 install git+git://github.com/PyCav/jupyterhub-raven-auth.git

## Configuration

Configure by adding:

```python
c = get_config()

from raven_auth.raven_auth import RavenAuthenticator
c.JupyterHub.authenticator_class = RavenAuthenticator

c.RavenAuthenticator.description = "pyCav"
c.RavenAuthenticator.long_description = "Welcome to the pyCav Jupyterhub server."
c.RavenAuthenticator.login_logo = '/absolute/path/to/logo/file'
```

## Whitelisting

The plugin uses the [Python3 ibisclient](https://www.lookup.cam.ac.uk/doc/ws-doc/) to interface with the University Lookup Service (ULS).
The jupyterhub-raven-auth plugin does not provide any configuration options to provide a username and password to access the ULS.
As such, access is *Anonymous* by default. This requires that the server running JupyterHub be inside the Cambridge University Data Network (CUDN).

To let the plugin know that it is operating within the CUDN, use the configuration option:

```python
c.RavenAuthenticator.inside_cudn = True
```

The allowed colleges are provided as a Set. So for example, to only allow Christ's College Postgraduates **or** members of the Department of Physics use the configuration option:

```python
c.RavenAuthenticator.allowed_colleges = {'PHY','CHRSTPG'}
```

## LICENCE

This code released under the [BSD License](https://github.com/PyCav/jupyterhub-raven-auth/blob/master/LICENSE).


