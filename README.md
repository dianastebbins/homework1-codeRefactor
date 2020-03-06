# homework1-codeRefactor

## Project Description
Use html and css skills learned in Week One of Coding Bootcamp to refactor an existing webpage of Horiseon Social Solution Services, Inc. to make it better accessible, reduce code redundancy and correct any errors.

## Table of Contents
* [Changes Made in index.html](#changes-made-in-index.html)
    *[Semantic](#semantic)
    *[Redundancy Reduction](#redundancy-reduction)
    *[Accessibility](#accessibility)
    *[Bug Fix](#bug-fix)
    *[Other](#other)
* [Changes Made in style.css](#changes-made-in-style.css)
    *[Match Semantic html Changes](#match-semantic-html-changes)
    *[Redundancy Reduction 2](#redundancy-reduction-2)
    *[Other 2](#other-2)
* [User Story and Acceptance Criteria](#user-story-and-acceptance-criteria)
    * [User Story](#user-story)
    * [Acceptance Criteria](#acceptance-criteria)
* [Installation](#installation)
* [Usage](#usage)
* [Installation](#installation)
* [Credits](#credits)
* [License](#license)
* [Badges](#badges)
* [Contributing](#contributing)
* [Tests](#tests)

## Changes Made in index.html
### Semantic
1. changed **div class="header"** and **div class="footer"** tags to **header** and **footer** tags, respectively
2. changed **div** tag holding list elements to **nav** tag
3. changed **div** of **div class="hero"** to **figure**
    * also changed **class="hero"** to **id="hero"** because "hero" seems more like a particular instance rather than a reusable class
4. changed **div class="content"** tag to **content** tag
5. changed **div class="benefits"** tag to **aside** tag
### Redundancy Reduction
6. changed **div**s with class identified as search-engine-optimization, online-reputation-management, and social-media-marketing to **section**s with **class="content-section"**
7. changed **div**s with class identified as benefit-lead, benefit-brand, and benefit-cost all to **section**s with **class="benefits-section"**
### Accessibility
8. replaced **title** text with "Info page for Horiseon Social Solution Services, Inc."
9. added **alt="[description]"** inside **img** tags (6)
### Bug Fix
10. added **id="search-engine-optimization"** to Search Engine Optimization **section** so the **href="#search-engine-optimization">Search Engine Optimization** link would work
### Other
11. changed **footer h2** to **h4** (default behavior) to keep headers in descending order down page/content
12. updated copyright at bottom to reflect year 2020
13. added some comments

## Changes Made in style.css
### Match Semantic html Changes
1. changed **.header** and **.footer** definitions to **header** and **footer**, respectively
2. changed **header div** definition to **nav**
3. changed **.hero** to **#hero** to match html change
4. changed **.content** definition to **content**
5. changed **.benefits** definition to **aside**
### Redundancy Reduction 2
6. combined redundant class stylings into single styling
    1. combined **.search-engine-optimization**, **.online-reputation-management** and **.social-media-marketing** into a single **.content-section**
    2. combined **.benefit-lead**, **.benefit-brand**, and **.benefit-cost** into a single **.benefits-section**
    3. **.search-engine-optimization h2**, **.online-reputation-management h2**, and **.social-media-marketing h2** combined into just **h2**
    4. **.benefit-lead h3**, **.benefit-brand h3**, and **.benefit-cost h3** combined into just **h3**
    5. **.search-engine-optimization img**, **.online-reputation-management img**, and **.social-media-marketing img** combined into a single **.content-section img**
    6. **.benefit-lead img**, **.benefit-brand img**, and **.benefit-cost img** combined into a single **.benefits-section img**
7. changed unnecessary path-like .css definition names to direct element or class definitions
    1. **header h1** to just **h1**
    2. **header h1 .seo** to just **.seo**
    3. **header div ul li** to just **li**
### Other 2
8. removed **header div ul** because the **list-style-type: none;** content appears to be redundant when using the **display: inline-block** attribute in the **li** styling.
9. removed **footer h2** (using default **h4** tag in html instead)
10. reordered code into order that makes sense to me: elements then classes then ids, more or less in the order each type appears in the html (not a rule, just a starting guideline :-)  

## User Story and Acceptance Criteria 
    * (copied from Homework instructional README.md, for reference)
### User Story
AS A marketing agency

I WANT a codebase that follows accessibility standards

SO THAT our own site is optimized for search engines

### Acceptance Criteria
GIVEN a webpage meets accessibility standards

WHEN I view the source code

THEN I find semantic HTML elements

WHEN I view the structure of the HTML elements

THEN I find that the elements follow a logical structure independent of styling and positioning

WHEN I view the image elements

THEN I find accessible alt attributes

WHEN I view the heading attributes

THEN they fall in sequential order

WHEN I view the title element

THEN I find a concise, descriptive title

## Installation
## Usage
## Credits
User Story and Acceptance Criteria copied from provided Homework files of Full Stack Coding Bootcamp.
## License
## Badges
## Contributing
## Tests
