Chy Auth for Sentry
======================

An SSO provider for Sentry which enables Chy Apps authentication.

Install
-------

$ pip install sentry-auth-chy

Setup
-----

Start by `creating a project in the Chy Developers Console`_.

Then, create an OAuth Client ID/Secret pair via `Project Credentials`_.

In the **Authorized redirect URIs** add the SSO endpoint for your installation::

    https://sentry.example.com/auth/sso/

Finally, obtain the API keys and plug them into your ``sentry.conf.py``:

.. code-block:: python

    CHY_CLIENT_ID = ""

    CHY_CLIENT_SECRET = ""

