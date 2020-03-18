---
description: Everything you need to know about customising hs_auth for a Hackathon
---

# hs\_auth

## Prerequisites

Before you start modifying for your hackathon, you need to have the following projects setup. Please follow their respective guides on Github for further instructions.

* [hs\_auth](https://github.com/unicsmcr/hs_auth)

## Required Edits

### .env

* Change `MONGO_PASSWORD` to something unique
* Change `JWT_SECRET`
* Set `APPLICATION_URL`
* Set `AUTH_URL`
* `SENDGRID_API_KEY`

### mongo.env and mongo\_express.env

* Change MONGO\_INITDB\_ROOT\_PASSWORD \(in `mongo.env`\)
* Change ME\_CONFIG\_MONGODB\_ADMINPASSWORD \(in `mongo_express.env`\) to the value same as `MONGO_INITDB_ROOT_PASSWORD`

### templates/emails

This is where it gets a bit trickier, these files are a bit hard to edit, but just look for the lines listed

#### emailVerify\_email

* Line 134, defines logo shows at top of email
* Line 198, Facebook link
* Line 199, Twitter link

#### passwordReset\_email

* Line 134, defines the logo at the top of email
* Line 196, Facebook link
* Line 197, Twitter link

### static/img

* favicon.ico

### config/

#### base.yaml

* name \(Full name of the hackathon, e.g. GreatUniHack 2020\)
* email
* app\_url \(Domain at which the application can be accessed, **including** subdomain\)
* data\_policy\_url

#### production.yaml

* domain\_name \(Domain of the hackathon, **excluding** subdomain\)

