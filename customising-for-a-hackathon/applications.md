---
description: Everything you need to know about customising hs_application for a Hackathon
---

# hs\_application

## Prerequisites

Before you start modifying for your hackathon, you need to have the following projects setup. Please follow their respective guides on Github for further instructions.

* [hs\_auth](https://github.com/unicsmcr/hs_auth)
* [hs\_applications](https://github.com/unicsmcr/hs_application)

## Required Edits

### .env

* Change `DB_PASSWORD` to something unique
* `APPLICATION_URL`
* `AUTH_URL`
* `DROPBOX_API_TOKEN`
* `SENDGRID_API_KEY`

{% hint style="info" %}
You only need to set `DROPBOX_API_TOKEN` if you plan on using CVs
{% endhint %}

### src/settings/

* hackathon.json
* questions.json

### public/img

* Favicon
* Logo





