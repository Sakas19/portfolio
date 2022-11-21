Hi Sharvnaz!

Nice work!

As you can see below you've ticked most of the boxes. I've added a few comments below about things I would like fixed up. It's mainly about organising the files and code

Would you please make the changes, then push to github and let me know when it is done so I can have another look?

*************************************

CRITERIA FOR GRADING

*************************************

GODKÄNT:
-------------------------------------

3 separate pages: ✅

A header with a page title on every page: ❌
  "Project" has a title, but none of the other pages. Google expects each page to have a unique h1.
  Be careful using % for padding etc when the element is a child of body. % takes their value from the parent - in styles.css the header has 1% top and bottom. This turns into 1% of the height of the body, and because different pages have different content, the body will be diferent heights. For example, the body on the about-me page is 3 times as largge as the body on the projects page - this means the padding in the header is larger on the about-me page. You can notice the different when changing pages.

A navigational menu every page with links to the other pages: ✅

Contact form:
    Email: ✅
    Message: ✅
    Required: ❌
    Mail to: ✅
      Need to add the attribute "required" to each input

RWD:
    Desktop: ✅
    Mobile: ✅
     Menu gets a bit misaligned on mobile view

External CSS: ✅

-------------------------------------

VÄLGODKÄNT:
-------------------------------------

Current page indication in the menu: ❌
  The way to fix this is to add a class - for example "active" - on the relevant menu item for each page, and add some styling to that class

Responsive Image: ✅

RWD:
  Media Query: ✅
    Probably could use this for styling the mobile menu
  Flex/Grid: ✅

Separate CSS: ✅ ❌
  You should have a "css" or "styles" directory that holds all your style sheets
  Although you do use separate css files, there is dublicated contetn inside them. For example the header and navigation styling classes - .header and .navbar - are in all 3 css files (and it looks like all the navbar styling is repeated twice in styles.css!)
  Common elemnts like the header and navigation should be inside one "general" file such as styles.css, then that file should be imported in each html file.
  Individual pager stylesheets should only have the styles that are either unique or different on those pages. 
  This might mean you have very short css files, and that is the preferred way. It makes it very asy to find the specific styles for a specific class.
  Semantic: ✅

Semantic Element naming: ✅
  Same as with css, all the html should bbe inside an html directory. Images shoul be in an images directory.

Code Style:
  HTML: ✅ ❌
   General good, though the indentation is a bit messed up. It should have a consistent 2 or 4 space indentation
   text.html is missing an opening body tag, while  projects has 2 opening body tags! 
  CSS: ✅
    Very nice!