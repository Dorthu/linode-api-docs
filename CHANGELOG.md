# Change Log
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

## [Unreleased]

## [0.16.2] 2017-12-11
### Added
- Deprecation flags (#2756, #2821)
- /account/payments/paypal and /account/payments/paypal/execute (#2801)
- /domain/clone (#2747)

### Changed
- renames /linode/volumes to /volumes (#2754)
- /distributions are now in /images (#2822, #2823, #2815)
- API Changelog updated for 2017-12-11 release

## [0.16.1] 2017-12-01
### Fixed
- Docs rendering in mobile used roughly half-width since 0.16.0 (#2796)

## [0.16.0] 2017-11-29
### Changed
- Update docs page titles (#2753)
- Document payment "usd" as String
### Added
- Documented all enum fields (#2464)
- Document Distribution ID
### Fixed
- Scroll content when clicking on a subnav item (#2733)
- Allow nav to scroll with a short window (#2734)

## [0.15.0] 2017-11-20
### Changed
- Grants have been reworked
### Added
- API Changelog for 2017-11-20
- CAA domain record properties are documented
- Payment properties are documented
### Fixed
- Many more example values are provided
- Many typos in property defintions have been corrected

## [0.14.1] 2017-11-05
### Fixed
- Numerous missing types and descriptions were added
- Oauthclient type was incorrectly called Client
- Nodebalancer Config did not document certificate parameteres correctly
- Nodebalancer and SupportTicket had undocumented response properties

## [0.14.0] 2017-10-23
### Changed
- /account/payments "amount" is now a string
### Added
- /user/:id/grants GET includes "longview" and "images"
- /profile/grants GET includes "longview" and "images"
- /images GET
- /images/:id GET, PUT, and DELETE
- /linode/instances/:id/disks/:id/imagize POST
- /linode/instances POST now accepts "image"
- /linode/instances/:id/rebuild POST now accepts "image"
- /account/notifications GET
- /account/settings GET and PUT now includes "longview\_subscription"
- /longview/subscriptions GET
- /longview/subscriptions/:id GET
- /longview/clients GET and POST
- /longview/clients/:id GET, PUT, and DELETE

## [0.13.3] 2017-10-10
### Changed
- obtaining token docs #2555
### Fixed
- Fix spacing near changelog alert #2613
- README links should be relative #2557
- ipv6 networking typos #2556

## [0.13.2] 2017-10-04
### Changed
- Endpoint docs for pricing, disks, config, volume, oauthclient
### Added
- Changelog for 2017-10-04
- documentation for account/credit-card
- documentation for account/payments
- documentation for linode/volumes/:id/clone
- documentation for profile/apps


## [0.13.1] 2017-09-28
### Fixed
- Request parameters should render required/optional labels

## [0.13.0] 2017-09-26
### Added
- Add a sidebar (#2494)
### Changed
- Use Yarn rather than NPM (#2520)
- removed extraneous "\_" from properties
- Show more of example up front
- Smarter height on collapsed examples

# [0.12.6] 2017-09-20
### Added
- Changelog page

# [0.12.5] 2017-09-19
### Added
- changes to document api release

# [0.12.4] 2017-09-18
### Fixed
- regression after API breaking changes #2548

# [0.12.3] 2017-09-18
### Added
- documentation for API breaking changes #2547

# [0.12.2] 2017-08-30
### Fixed
- remember scroll history and # jump links work #2486

# [0.12.1] 2017-08-30
### Fixed
- missing docs GET responses in many pages #2486

# [0.12.0] 2017-08-29
### Added
- documentation for mutate #2471
- documentation for stats #2472
- more debugging on yaml failure #2371
### Changed
- removed old/unused anchor tags #2333
- updated python docs for region and type #2362
### Fixed
- breakage on long endpoints on mobile #2420

## [0.11.4] 2017-08-14
### Fixed
- volume documentation together and at the correct endpoints

## [0.11.3] 2017-08-08
### Changed
- switch to _id for fields that expect an integer id #2385

## [0.11.2] 2017-08-08
### Added
- docs for linode clone endpoint #2399

## [0.11.1] 2017-08-04
### Changed
- /account/profile -> /profile and other api followups #2373

## [0.11.0] 2017-08-01
### Added
- added more debugging for failing prebuild script #2233
- added docs linting #2283
- added developers links to docs readme #2289
- add response_type to oauth client docs #2330
- add additional oauth fields #2334
### Changed
- show paginated results on paginated endpoints #2279
- no custom object names #2279
- independent method response fields #2320
- scopes to scope for requesting scopes in oauth #2331
### Fixed
- sets non-integer numbers correctly to be float #2279
- fixed typo in python example #2298

## [0.10.2] 2017-07-20
### Fixed
- account endpoint documentation #2318

## [0.10.1] 2017-07-17
### Fixed
- python docs domain field naming #2281

## [0.10.0] 2017-07-10
### Added
- missing /networking responses #2184
- missing Linode backups response #2184
- see also links for relevant objects #2190
- full support for grouping endpoints on index pages #2194
- prebuild to server start, updated readme with build steps #2217
- block storage get docs #2225
- endpoints for removing public IPv4 addresses #2226
### Removed
- duplicate clients yaml #2176
- drop miniheader #2231

## [0.9.1] 2017-06-29
### Fixed
- fix multiple docs/src/components/tables/cells directories

## [0.9.0] 2017-06-29
### Added
- page titles for each page #2114
- next link for guides #2098
- expandable icon for expandable table rows #2121
- show active sidebar nav item #2115
### Changed
- improvements to rendering on mobile #2156
- LinodeClient example docs updated #2137
- misc Python doc updates #2020
- endpoints sorted alphabetically #2148
- cleanup Python docs build step #2144
### Fixed
- no clipboard on errors examples #2167

## [0.8.0] 2017-06-16
### Added
- info block to the docs intro which points to testing with cURL and how to get started with a PAT #2072
- OAuth scope denotation to endpoint methods throughout the docs #2075
- introductory python guides #2085
- python wrapper API documentation #2085
### Changed
- reorganized guides into guides and libraries, cURL and python guides now exist on the same index #2085
### Fixed
- missing method response field and method request param types denotations #2070
- a couple links in creating a Linode cURL guide #2090

## [0.7.3] 2017-06-09
### Added
- added linode_kvmify to account/events action enums
### Changed
- account/events action enums renamed from dns > domain
- renamed domains display_group to group

## [0.7.2] 2017-06-09
### Changed
- reorganized routes and added index redirect from /v4/ to /v4/introduction

## [0.7.1] 2017-06-09
### Changed
- distribution "recommended" renamed to "deprecated"

## [0.7.0] 2017-06-08
### Added
- required and optional denotation to method params
- collapsed by default and toggle for response examples

## [0.6.0] 2017-06-07
### Added
- Syntax highlighting for code examples
- Copy to clipboard icons for examples
### Fixed
- added missing cost indicators to methods

## [0.5.2] 2017-06-07
### Fixed
- added missing Authenticated denotations with icons to endpoints

## [0.5.1] 2017-06-07
### Fixed
- Made the $api_root and $version variables from yaml render to the constants in the prebuild step

## [0.5.0] 2017-06-06
### Added
- cURL guide #1878
### Fixed
- updated duplicate base version vars to use API_VERSION, prebuild script uses environment var if present
- include original /reference redirect to the new /v4/introduction #2019
### Changed
- updated Introduction section #2008

## [0.4.0] 2017-06-05
### Added
- /v4 to the base of all urls

## [0.3.2] 2017-06-02
### Fixed
- examples typo in linode/instances/:id/ips/sharing, which caused a page break

## [0.3.1] 2017-06-01
### Fixed
- temporary fix for `npm run prebuild` incorrect reference

## [0.3.0] 2017-05-31
### Added
- .gitignore file #1970
- /reference default redirect to /introduction #1958
### Changed
- json removed and yaml added in it's place #1909
- docsConvert.js renamed to prebuild.js and prebuld defined as an npm script #1909
- api /objects read and conversion moved from objectsConvert.js (deleted) to prebuild.js #1909
- src/api.js, which is now ignored since it's built #1970
- increased with on endpoint index table headers for longer urls #1968
### Fixed
- broken /reference crumbs #1963
- broken /linode/types and /linode/types/:id endpoints #1964
### Removed
- transform.sh no longer needed after yaml move #1909

## [0.2.1] 2017-05-26
### Fixed
- subtle tabs bug which caused tab content to not be rendered, python examples now show
- example formatting for arrays, some additional schema definitions in tables for the same arrays

## [0.2.0] 2017-05-23
### Added
- Nested object schemas and examples for method params and responses
- Nested enumerations for method responses
- Python guide section intro

### Fixed
- Missing response examples for GETs

## [0.1.1] 2017-05-17
### Fixed
- de-duped protocols in some urls since env vars provide the protocol with base urls at build time

## [0.1.0] 2017-05-17
### Added
- changelog file
