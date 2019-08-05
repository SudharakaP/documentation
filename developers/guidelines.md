---
description: Describes what we expect from new code written for our product
---

# Best Practice Guidelines

### General rules

* When adding new dependencies, we use [fixed versions](https://docs.npmjs.com/about-semantic-versioning).
* Don't commit `package-lock.json` if you're not making any changes to the libraries.

### Frontend rules

* The strings must be internationalized. See [/help/developers/translations](https://docs.opencollective.com/help/developers/translations)
* Whenever it's possible we must use `styled-components` to write styles. See [OC Styleguide](https://opencollective-styleguide.now.sh/)
* We're getting rid of `Bootstrap` and `material-ui`. Please don't use them for new developments.
* Icons must be imported from the [styled-icons](http://styled-icons.js.org/) library.
* Tests written with Cypress must follow our [good practices](https://docs.opencollective.com/help/developers/testing-with-cypress) conventions.

## Special tips

* If the issue you're working on require changes in both API and Frontend, give your Git branches the same name. CI will automatically pull the correct API's branch when testing the frontend.
