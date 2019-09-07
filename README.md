Auth provider
=============

A Haskell implementation of [OpenID Connect](http://openid.net/connect/).

Prerequisites
-------------
Instasll Haskell [stack](https://docs.haskellstack.org/en/stable/README/#how-to-install)

Building
--------

    $ git clone https://github.com/solutions-for-inventory/auth-provider.git
    $ cd auth-provider

Do stack setup only the first time

    $ stack setup

Build the project

    $ stack build

Config DB provider
-------------------

    Edit auth-provider/config/settings.yml

Run
-------------------
    $ stack exec auth-provider

Test Example
-------------------

    http://localhost:3000/oauth/authorize?client_id=app&state=state_code&response_type=code&redirect_uri=http%3A%2F%2Flocalhost:8080/app
