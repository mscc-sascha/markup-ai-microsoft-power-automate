# Markup AI Content Guardian Agents

Markup AI gives you the tools to build content governance into any workflow, so your content is always clear, on-brand, and compliant before it ever sees the light of day.

For more details, have a look at our [public documentation](https://docs.markup.ai/overview)

## Prerequisites

You will need the following to proceed:

* A Microsoft Power Apps or Power Automate plan with custom connector feature
* Get your Markup AI API Key 
    * [Get access](https://auth.markup.ai/u/signup) 


## Supported Operations

The connector supports the following operations:

### Style Guides

* `List Style Guides` Retrieve all style guides associated with your organization.
* `Create Style Guide` Create a new style guide that can be used in checks, suggestions, and rewrites.
* `Get Style Guide` Retrieve a specific style guide by ID.
* `Update Style Guide` Update the name of an existing style guide.
* `Delete Style Guide` Delete a style guide by ID.

### Style Check

* `Create Style Check` Analyze text for grammar, style, and clarity issues.
* `Get Style Check` Retrieve style check results.

### Style Rewrite

* `Create Style Rewrite` Rewrite text with style corrections applied.
* `Get Style Rewrite` Retrieve rewrite results.

### Style Suggestion

* `Create Style Suggestion` Get suggested corrections for text.
* `Get Style Suggestion` Retrieve suggestion results.

## Best Practices

* For the operations `Create Style Check`, `Create Style Suggestion` and `Create Style Rewrite` always define Webhook URL for the asynchronous response processing. Try not to use a polling mechanism.

## Known Issues and Limitations

Have a look at our [community](https://community.markup.ai/) to stay up to date with features and questions.
