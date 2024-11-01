# API Guidance
API Guidance is text and videos that is tagged and aligned with business, technical, policy, and people considerations, providing a specific piece of guidance that is aligned with the policies and rules being applied across governance, ensuring that teams who are producing or consuming APIs have what they need to guide them forward.

## API Commons
API Guidance are a new API Commons schema that is associated with API policies, which can then be bridged to API rules, providing Just-in-Time API Guidance for teams who are producing or consuming APIs, making sure business and technical stakeholders both have what they need in each individual moment across the entire API lifecycle.

## Example ([guidance-example-1](guidance-example-1.yml))

```
title: Change - Versioning
subtitle: Managing the change across APIs using versioning.
tags:
- Change
- Versioning
- Versions
author: kin
visibility: public
business: Change is an inevitable part of business.
technology: Versioning is done using Semantic Versioning.
policies: There are multiple policies governing versioning.
people: Versioning is about communicating change.
```

## JSON Schema ([guidance-json-schema](guidance-json-schema.yml))

```
"$schema": http://json-schema.org/2020-12/schema
type: object
description: Machine-readable guidance meant for humans to consume.
properties:
  title:
    type: string
    description: The title of the guidance being offered.
  subtitle:
    type: string
    description: A short summary of the guidance being offered.
  tags:
    type: array
    description: The key words or phrases applied to guidance.
    items:
    - type: string
  author:
    type: string
    description: The human author of the guidance.
  visibility:
    type: string
    description: Whether it is public or private.
  business:
    type: string
    description: The business implications of the guidance.
  technology:
    type: string
    description: What technology is involved with guidance.
  policies:
    type: string
    description: What policies apply to area of guidance.
  people:
    type: string
    description: What are the human impacts of this guidance.
required:
- title
- subtitle
- tags
- author
- visibility
- business
- technology
- policies
- people
```

# API Policies, Rules, Experience, and Guidance
API Guidance are associated with policies, which then can also provide the bridge to the rules used to lint the business and technical contracts in place for APIs, helping provide one-click access to the answers API producers and consumers will need as they work to deliver consistent APIs, and put APIs to work in applications and integrations.

<img src="https://kinlane-productions2.s3.us-east-1.amazonaws.com/policies-rules-guidance-experience-lifecycle.jpg">

This work acknowledges that services, tooling, and the general approach of API governance is only using rules applied to OpenAPI, which is beginning to expand to AsyncAPI, GraphQL, and Arazzo workflows, but is proposing the first schema for aligning this work with business objectives, when teams are ready for it.

## Support
This work is in early stage of development and rapidly moving as they are being applied in a variety of user interfaces and approaches to the automation and reporting of API governance. If you would like to contribute, have any questions, or would like to inform the work happening, please submit a GitHub issue on the repository or email kin@apievangelist.com.