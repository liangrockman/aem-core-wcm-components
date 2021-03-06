<!--
Copyright 2017 Adobe Systems Incorporated

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
-->
Page (v1)
====
Extensible page component written in HTL.

## Features
* Editable templates
* Page title, subtitle, description and thumbnail
* Navigation title, or hide from navigation
* Vanity URL, page alias and redirection
* Page tagging and define content language
* On/Off time and launches
* Blueprints and live copy
* Closed user groups and permissions
* Cloud services

### Use Object
The Page component uses the following use objects:
* `com.adobe.cq.wcm.core.components.models.Page`
* `com.adobe.cq.wcm.core.components.models.SocialMediaHelper`
* `com.day.cq.wcm.foundation.TemplatedContainer`

### Component policy configuration properties
The following configuration properties are used:

1. `./clientlibs` - allows to define a list of client libraries to be loaded by the pages associated to this configuraiton policy

### Edit dialog properties
The following properties are written to JCR for this Page component and are expected to be available as `Resource` properties:

1. `./jcr:title` - defines the title for this page
2. `pageName` - defines the page name for this page
3. `./cq:tags` - defines the tags for this page
4. `./hideInNav` - if set to `true` then this page will be hidden from navigation
5. `./pageTitle` - defines an alternate title for this page
6. `./navTitle` - defines the navigation title for this page
7. `./subtitle` - defines a subtitle for this page
8. `./jcr:description` - defines a description for this page
9.  `./onTime` - defines when the page should become available
10. `./offTime` - defines when the page should not be available any more
11. `./sling:vanityPath` - defines a vanity URL at which this page could be accessed
12. `./sling:redirect` - if set to `true`, then this page will redirect to its defined vanity URL
13. `./jcr:language` - defines the language set for this page, to help with `i18n`
14. `./cq:designPath` - defines where the design for this page is stored
15. `./sling:alias` - defines a Sling alias for this page, so that the page can be accessed at a different resource path
16. `./cq:allowedTemplates` - defines a template or a list of templates that the page should use
17. `./cq:exportTemplate` - defines the template used for exporting this page for content synchronisation
18. `./socialMedia` - defines the enabled social media configurations
19. `./variantPath` - allows defining the social media variation experience fragment to be used for generating page meta data for social
media
20. `./cq:contextHubPath` - defines the Context Path configuration used by this page
21. `./cq:contextHubSegmentsPath` - defines the Context Path Segments Path

## Information
* **Vendor**: Adobe
* **Version**: v1
* **Compatibility**: AEM 6.3
* **Status**: production-ready
* **Documentation**: [https://www.adobe.com/go/aem\_cmp\_page\_v1](https://www.adobe.com/go/aem_cmp_page_v1)

