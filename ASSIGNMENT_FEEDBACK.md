Updated 7-12-2022

Good Morning Sharvnaz!

Great work, thanks for taking the time to look at the feedback and make changes.

The only thing I would like you to do is to look at the indenting on the CSS.

Everything else is fine, so I'm happy to say you have met the requirements for a VG grade. Well done!

*************************************

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

A header with a page title on every page: ✅
  UPDATED 30-11-2022
  Great!

A navigational menu every page with links to the other pages: ✅

Contact form:
    Email: ✅
    Message: ✅
    Required: ✅ 1/2
    Mail to: ✅
      Need to add the attribute "required" to each input - email has it but not comment

RWD:
    Desktop: ✅
    Mobile: ✅
     Menu gets a bit misaligned on mobile view

External CSS: ✅

-------------------------------------

VÄLGODKÄNT:
-------------------------------------

Current page indication in the menu: ✅
 UPDATED 30-11-2022
  Fixed, looks good.

  The way to fix this is to add a class - for example "active" - on the relevant menu item for each page, and add some styling to that class

Responsive Image: ✅

RWD:
  Media Query: ✅
    Probably could use this for styling the mobile menu
  Flex/Grid: ✅

Separate CSS: ✅ Fixed! 7-12-2002
  The css itself is good, but needs to be organised a little bit better.

  The first thng is to create folders to hold the different kinds of files, so make an html folder for the html files, a css folder for css and an images folder.

  The move all the "common" styles - the styling that applies to every page - to a general.css file. In your css files, you are repeating things, eg the ::root { ... } element is in all 3 files, so is  .header, .logo, and .navbar and its related elements. By creating one general file for common eleemnts, you will be able to remove about 70 lines from each of the other 3 files

  Semantic: ✅

Semantic Element naming: ✅
  Same as with css, all the html should bbe inside an html directory. Images should be in an images directory.

Code Style:
  HTML: ✅ ❌
   General good, though the indentation is a bit messed up. It should have a consistent 2 or 4 space indentation
   
   For example,this  from contact-me.html:

   <h1 class="heading">Contact me</h1>
    <div class="form">
        <form action="mailto: Sarvnaz.kasaei@gmail.com" method="post">
            <div id="form-main">
            <div id="form-div">
              <p class="name">
                  <input name="name" type="text" class="feedback-input" placeholder="Name" id="name"/>
                </p>
  
  Should be indented like this using 4 indents on every new element:

  <h1 class="heading">Contact me</h1>
  <div class="form">
      <form action="mailto: Sarvnaz.kasaei@gmail.com" method="post">
          <div id="form-main">
              <div id="form-div">
                  <p class="name">
                      <input name="name" type="text" class="feedback-input" placeholder="Name" id="name"/>
                  </p>
  CSS: ✅
    Very nice! Theres a bit of inconsistent indentation and you should always have a space between the selector name and the opening

    With css the selector should always start at the first column of the page, and the closing } should be at the same level with all the properties indented 4 spaces - eg from styles-contact.css line 131:

  #name{
        background-color: white;
        background-size: 30px 30px;
        background-position: 11px 8px;
        background-repeat: no-repeat;
      }

      should be:

#name {
    background-color: white;
    background-size: 30px 30px;
    background-position: 11px 8px;
    background-repeat: no-repeat;
}