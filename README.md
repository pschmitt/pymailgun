pymailgunner
=========

A simple mailgun client

Installation
============

```
pip install pymailgunner
```

Usage
=====

To create a mailgun Client you will need a mailgun api key and the domain name
to use (must match the domain name registered on the mailgun website).

``` python
from pymailgunner import Client

mailgun_client = Client({api_key}, {domain_name})
```

Or, for domains in the EU Region, 

``` python
from pymailgunner import Client

mailgun_client = Client({api_key}, {domain_name}, eu_domain=True)
```

Features
========

To send an email

``` python

mailgun_client.send_mail(...) #see send_mail docstring
```
