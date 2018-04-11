# Indigo Developer Handbook

#### the cms ! a handy guide
- [preview and prod](#preview-and-prod)
- [widgets](#widgets)
	-[banners](#banners)
	-[html block](#html-block)
	-[content block](#content-block)
	-[html bundle](#html-bundle)
	-[product lists](#product-lists)
		- [tabbed carousels](#tabbed-carousels)
		- [list vs grid vs carousel view](#list-vs-grid-vs-carousel-view)
- [templates](#templates)
- [workarea vs extra tools](#workarea-vs-extra-tools)
- [history](#history)

#### who's who at indigo
- [merchndisers](#)
- [designers](#)
- [IT](#)
- [Online Production](#)
	- [Preben](#)
	- [Launa](#)
	- [Darshana](#)
	- [YOU](#)

#### handy terms
- [cta](#)
- [quicklinks](#)
- [banner](#)
- [merchie](#)
- [slice](#)

#### the work
- [maintaining regular styles vs merch site shops](#)
- [how to build a page](#)
- [french vs english](#)
- [site standards (styles and code)](#)

#### tools
- [hipchat](#)
- [Proworkflow](#)
- [photoshop](#)
- [avocode](#)
- [trello](#)
- [github](#)

## the cms ! a handy guide
Welcome to Indigo's CMS!
Online Production builds out pages within our CMS which is called Ektron. Ektron has a .NET backend and we have HEAVILY customized it in house. Indigo developers have been building out features for our needs for years at this point so it is kind of its own specific CMS. It has many quirks and specificities. 

### preview and prod
OP has access to a staging environment called *preview* and the live version of the site that we call *production* or *prod*. When you are working on developing a new project, page, or feature you will work in preview. preview is accessed when you are on the indigo network and enter `preview.` before any indigo URL. Here you will get a set of tools in a bar across the top of your screen.  `FILE`, `VIEW`, `PROPERTIES`, and `HELP`.

`FILE` has the options to 
*edit* which will open the page up for editing
*publish* which means send through to live site
*check-in* which means to save and update to preview site only
*cancel* which cancels changes you've made while in editing mode

`VIEW` will give links to the page either in (workarea or extra tools)(#workarea-vs-extra-tools) by clicking on properties

`PROPERTIES` gives you relevant info to the page you're on such as the most recent editor, ID, template, and its status `approved (A)`, `checked-in (I)`, or `pending(P)`.

`HELP` launhes the help page.

###widgets
Widgets are the building blocks of a page within our CMS. The following is a description of the ones you will be using most.

#####banners
Banners are the main way we get images on the site. Banners are designed by studio at the behest of merchandisers or elsewhere from within Indigo. There are banners that have live text and banners that have images of text. When the banner has live text it means that the merchandiser can change the text and images independantly. There are currently a few standard banners that have been set up.

	.swb => Standard Width Banner. Main banner on a page.
	.feat-list => A banner that takes of 50% of a standard layout and contains other banners inside as a list.
	.feat-list-inner + .feat-list-inner-a/.feat-list-inner-b/.feat-list-inner-c => Inner banners inside featured lists usually containing a single product or idea. a/b/c denotes whether banner is 1st, 2nd, or 3rd.
	.feat-prod + .feat-prod-l/.feat-prod-r => A banner that takes of 50% of a standard layout and also designation of whether is it on the right or left side of the page.
	.feat-promo => Skinny banner that goes 100% of the width of a standard layout
	.eb => Editorial blocks. 3 across banners at the bottom of many merchandised pages.

		Some classes that are used on individual banners in the field *Caption Custom Class*
		.swb-multi-cta / .swb-one-cta => Whether CTAs will all line up and be same width or if there is one button and there will just be 30px of space on the left and right sides of the text
		.feat-prod-centered / .feat-prod-70 / .feat-prod-heather / .feat-prod-2ctas => Denotes alternative feat-prod stylings. Can currently be viewed on Gifts page, Books dept page, Heather’s Picks, and Teen Books, respectively
		.white => Whether text will be white
		.gm / .books / .kids / .baby / .bargain => Denotes what department banner is used in. Will be used to do things like change all books pages underlines to a certain colour etc etc

		Some classes are used on individual fields on banners
		.cta => A call to action that is bold text with an arrow afterwards. No box
		.cta—button => A call to action that had a box around it and is a button.
		.cta—special => A call to action that is third in the list of three consecutive CTAs that is highlighted differently. Generally, it is the SHOP ALL button.

### workarea vs extra tools








