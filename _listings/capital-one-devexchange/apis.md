---
name: Capital One DevExchange
x-slug: capital-one-devexchange
description: What unites us all is a desire to create better end customer experiences.
  Were building a full suite of tools and technology that make essential things in
  peoples everyday life &ndash; money, finances, identity &ndash; simpler for you.
  Now is the time to join our beta program, and help us shape the future.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Purchases
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/purchases/master/_listings/capital-one-devexchange/apis.md
specificationVersion: "0.14"
apis:
- name: Capital One DevExchange Get all purchases
  x-api-slug: capital-one-devexchange
  description: Returns the purchases that you are involved in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}/purchases
  tags: Banks,Accounts, , Purchases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/purchases/master/_listings/capital-one-devexchange/accountsidpurchases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/purchases/master/_listings/capital-one-devexchange/accountsidpurchases-get-openapi.md
- name: Capital One DevExchange Create a purchase
  x-api-slug: capital-one-devexchange
  description: Creates a purchase where the account with the ID specified is the payer.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}/purchases
  tags: Banks,Accounts, , Purchases
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/purchases/master/_listings/capital-one-devexchange/accountsidpurchases-post-openapi.md
- name: Capital One DevExchange Get purchase by id
  x-api-slug: capital-one-devexchange
  description: Returns the purchase with the specific id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////purchases/{id}
  tags: Banks,Purchases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/purchases/master/_listings/capital-one-devexchange/purchasesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/purchases/master/_listings/capital-one-devexchange/purchasesid-get-openapi.md
- name: Capital One DevExchange Delete a specific existing purchase
  x-api-slug: capital-one-devexchange
  description: Deletes the specific purchase
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////purchases/{id}
  tags: Banks,Purchases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/purchases/master/_listings/capital-one-devexchange/purchasesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/purchases/master/_listings/capital-one-devexchange/purchasesid-delete-openapi.md
- name: Capital One DevExchange Update a specific existing purchase
  x-api-slug: capital-one-devexchange
  description: Updates the specific purchase
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////purchases/{id}
  tags: Banks,Purchases
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/purchases/master/_listings/capital-one-devexchange/purchasesid-put-openapi.md
- name: Capital One DevExchange Get all purchases by merchant
  x-api-slug: capital-one-devexchange
  description: Returns the purchases that a merchant is involved in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////merchants/{id}/purchases
  tags: Banks,Merchants, , Purchases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/purchases/master/_listings/capital-one-devexchange/merchantsidpurchases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/purchases/master/_listings/capital-one-devexchange/merchantsidpurchases-get-openapi.md
- name: Capital One DevExchange Get all purchases by account and merchant
  x-api-slug: capital-one-devexchange
  description: Returns the purchases that a merchant is involved in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////merchants/{id}/accounts/{accountId}/purchases
  tags: Banks,Merchants, , Accounts, Account, Purchases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/purchases/master/_listings/capital-one-devexchange/merchantsidaccountsaccountidpurchases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/purchases/master/_listings/capital-one-devexchange/merchantsidaccountsaccountidpurchases-get-openapi.md
- name: Capital One DevExchange
  x-api-slug: capital-one-devexchange
  description: What unites us all is a desire to create better end customer experiences.
    Were building a full suite of tools and technology that make essential things
    in peoples everyday life &ndash; money, finances, identity &ndash; simpler for
    you. Now is the time to join our beta program, and help us shape the future.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com//
  tags: Purchases
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/purchases/master/_listings/capital-one-devexchange/openapi.md
x-common:
- type: x-authentication
  url: https://developer.capitalone.com/platform-documentation/authorization-with-oauth-20/
- type: x-blog
  url: https://developer.capitalone.com/blogs/
- type: x-developer
  url: https://developer.capitalone.com/
- type: x-documentation
  url: https://developer.capitalone.com/platform-documentation/
- type: x-errors
  url: https://developer.capitalone.com/platform-documentation/errors/
- type: x-getting-started
  url: https://developer.capitalone.com/platform-documentation/getting-started/
- type: x-github
  url: https://github.com/capitalone
- type: x-website
  url: http://capitalone.com
- type: x-open-source
  url: https://developer.capitalone.com/open-source/
- type: x-sandbox
  url: https://developer.capitalone.com/platform-documentation/using-the-sandbox/
- type: x-login
  url: https://developer.capitalone.com/sign-in/
- type: x-selfservice-registration
  url: https://developer.capitalone.com/sign-up
- type: x-support
  url: https://developer.capitalone.com/support/
- type: x-privacy-policy
  url: https://www.capitalone.com/identity-protection/privacy/statement
- type: x-terms-of-service
  url: https://developer.capitalone.com/single/terms-and-conditions/
- type: x-twitter
  url: https://twitter.com/CapitalOneDevEx
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---