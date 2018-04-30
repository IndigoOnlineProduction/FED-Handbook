# Indigo Developer Handbook

#### the cms ! a handy guide
- [preview and prod](#preview-and-prod)
- [widgets](#widgets)
	- [banners](#banners)
	- [html block](#html-block)
	- [content block](#content-block)
	- [html bundle](#html-bundle)
	- [product lists](#product-lists)
		- [carousel vs list vs grid view](#carousel-vs-list-vs-grid-view)
		- [tabbed carousels](#tabbed-carousels)
- [templates](#templates)
- [workarea vs extra tools](#workarea-vs-extra-tools)
- [history](#history)

#### who's who at indigo
- [merchandisers](#merchandisers)
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
- [Akamai](#Akamai)
- [What’s Upload](#Whats-Upload)
- [Adobe Test & Target](#Adobe-Test-&-Target)
- [Jira](#Jira)
- [Confluence](#Confluence)
- [Endeca Lookup](#Endeca-Lookup)

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

### widgets
Widgets are the building blocks of a page within our CMS. The following is a description of the ones you will be using most.

##### banners
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

##### html block 
An HTML block is a widget that will accept HTML, CSS, and JS and lives and is localized only to that page. Wherever the widget is placed in the page that is the order where the code will be placed in the DOM. Wrap CSS in `<style>` tags and JS in `<scrip>` tags.

##### content block
Content block widgets are blocks of code that live on the cms and exist independantly of any page. Content blocks can be put on as many pages as you like and are generally used to repeat code or place code on a page that will be updated independatly of the page. Wrap CSS in `<style>` tags and JS in `<scrip>` tags.

##### html bundles
HTML Bundles function in almost the same way as content blocks but the HTML, CSS, and JS are seperated in the file and then minified and placed in the head of the page that they are placed on and are generally much more performant. `CMD` + `CTRL` + arrows moves you left and right between the files.

##### product lists
Product lists are pulled in either by a product list ID number or an Endeca ID. There are many configureable options within a product list including how many products to bring in and if they are within a range, and also what format they will display in:

###### carousel vs list vs grid view
These are the three views you can select from within the product list widget.
Carousel will show as many products as fit widthwise in one line with arrows on either side to scroll through.

### workarea vs extra tools

### Who's Who

#### merchandisers
	- Kim Gardiner: Senior Director of Online Content	
	- Seema Maloni: Senior Manager, Content
	- Aney Mei: Manages home page updates and campaigns
	- Stephanie Andrews: Merchandiser GM
	- Stephanie Clark: Manager GM merchandising
	- Michael Bacal: Manager of Book merchandising
	- Michael Gallagher: Special Promotions and Deals of the Week
	- Kaito McVey: Kids & Toys
	- Kalyn Cherney: Coordinator - GM
	- Josh Fehrens: Coordinator, Part time
	- Estelle Bresson: French Merchandiser
	
#### designers
	- Leanna Palmer - Creative Director
	- Katerina Slinkina - Project manager
	- Alisha Catellan - Project manager
	- Tomo Kato - Manager, Digital creative - she's the go to for any UI questions
	- Grainne McCarthy - Designer
	- Claudia Urquieta - Designer
	- Heidi Barett - Designer - Kids
	- Nicole Charles - Designer
	- Candice Lin - Designer
	- Adam Balsam - Designer - Emails
	- Frank Franz - UI Designer
	- Emily Dalton - UI Designer







