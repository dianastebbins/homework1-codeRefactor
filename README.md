# homework1-codeRefactor
Refactor an existing webpage for Horiseon Social Solution Services, Inc. to make it accessible

# Changes made to improve semantics, accessibility and performance of index.html
1. replaced **title** text with "Info page for Horiseon Social Solution Services, Inc."
2. added **alt="[description]"** inside **img** tags (6)
3. added **id="search-engine-optimization"** to Search Engine Optimization **content div** so the **href="#search-engine-optimization">Search Engine Optimization** link would work
4. changed **div class="header"** and **div class="footer"** tags to **header** and **footer** tags, respectively
5. added **class="horizontal-menu"** to **div** tag holding list elements
6. changed **div**s with class identified as benefit-lead, benefit-brand, and benefit-cost all to **div**s with **class="benefits-section"**
7. changed **div**s with class identified as search-engine-optimization, online-reputation-management, and social-media-marketing to **div**s with **class="content-section"**
8. changed **div class="hero"** to **div id="hero"** because "hero" seems more like a particular instance rather than a whole class
9. added some comments
10. updated copyright at bottom to reflect year 2020
11. changed **footer h2** to **h4** (default behavior) to keep headers in descending order down page
12. reordered code into order that makes sense to me: elements then classes then ids, more or less in the order each type appears in the html (not a rule, just a starting guideline :-)  

# Changes made in style.css to match any index.html changes and to reduce redundancy in style.css
1. changed **.header** and **.footer** definitions to **header** and **footer**, respectively
2. changed unnecessary path-like .css definition names to direct element or class definitions
    1. **header h1** to just **h1**
    2. **header h1 .seo** to just **.seo**
    3. **header div** to **.horizontal-menu**
    4. **header div ul li** to just **li**
3. removed **header div ul** because the **list-style-type: none;** content appears to be redundant when using the **display: inline-block** attribute in the **li** styling.
4. combined redundant class stylings into single styling
    1. **.search-engine-optimization h2**, **.online-reputation-management h2**, and **.social-media-marketing h2** combined into just **h2**
    2. **.benefit-lead h3**, **.benefit-brand h3**, and **.benefit-cost h3** combined into just **h3**
    3. **.benefit-lead**, **.benefit-brand**, and **.benefit-cost** combined into a single **.benefits-section**
    4. **.benefit-lead img**, **.benefit-brand img**, and **.benefit-cost img** combined into a single **.benefits-section img**
    5. **.search-engine-optimization**, **.online-reputation-management**, and **.social-media-marketing** combined into a single **.content-section**
    6. **.search-engine-optimization img**, **.online-reputation-management img**, and **.social-media-marketing img** combined into a single **.content-section img**
5. removed **footer h2** (using default **h4** tag in html instead)
6. changed **.hero** to **#hero** to match html change

# User Story and Acceptance Criteria copied from Homework instructional README.md for reference
## User Story
AS A marketing agency
I WANT a codebase that follows accessibility standards
SO THAT our own site is optimized for search engines

## Acceptance Criteria
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
