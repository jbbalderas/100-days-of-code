# 100 Days Of Code - Log

### Day 0: June 26 - July 5; 2018

**Today's Progress**: 
**Thoughts:** 

**Link to work:** [Tribute Page](https://learn.freecodecamp.org/responsive-web-design/responsive-web-design-projects/build-a-tribute-page)

### Day 1: July 6, Friday

**Today's Progress**: ...

**Thoughts** I've recently started coding,...

**Link(s) to work** [Tribute Page deployed online](https://jim-rohn.netlify.com/)

### Day 2: July 7, Saturday

**Today's Progress**: ...

**Thoughts** I've recently started coding,...

**Link(s) to work** [Tribute Page deployed online](https://jim-rohn.netlify.com/)

### Day 3: July 9, Monday

**Today's Progress**: ...

**Thoughts** I've recently started coding,...

**Link(s) to work** [Tribute Page deployed online](https://jim-rohn.netlify.com/)

### Day 4: July 10, Tuesday

**Today's Progress**:

```
1.09p
	Learned diff CSS Selectors:
		three normal: element, class, id
		star 				* 		{}
		descendant 			ul lu 	{}
		adjacent/beside 	h3 + ul {}
		attrib 	 	input[type] 	{}
		nth-of-type  ul:nth-of-type(even) {}

		~colt steele's WDBC c.5 039

		sibling 			h3 ~ p 	{}
		HTML5 CSS3 advance feature: 		a[href *= "google"]
			*= 	all including this word
			^=  all beginning with this word
			$=  all ending with this word
			~= 	has the value "" between two spaces
			|= 	has the value "" between two hypens / "" separated by hypen

		~rob percival's TCWD2 c.11 256
		sibling following 	h3 ~ p 	{}
		ImmediateDescendant ul>lu 	{}

	Learned CSS resets 	(myers, normalize, sanitize, todd-mcleon's)
	Learned relationship of "margin: 0 auto" + display properties (inline, block)
		-This solved my problem of a centered img inside an anchor tag but the white space is also being clickable :D
		~todd mcleon's HtCaW:aHTaCT c.9 *

2.23p
	problem -> display: flex not working on pic.div. Need to make the 'quote-container' and 'pic.div' flexed side by side with 'pic.div' as basis on right.
		solved: the FLEX must be on the desired elements' parent container div I want to be flexed. 
4.50p
	Learned about Flex-> FLEX-WRAP (default/none vs wrap vs wrap-reverse | one line vs multi vs flex-direction reversed)
	
5.53p break; problem -> w/o max-height w/ absolute px, pic-div height grows to max, 
	
9.19p 	solved: 1] flex 75% 25% expected ratio : flex: 3 &&/+ flex:1 solves this
				2] pic-div not respecting its parent container height : flex:1 (25%) ratio solved this too. ugh
				3] pic-div img vertical center : img{object-fit:contain} + *remove* pic-div{height:100%} 

Learned that flexbox and grid are now and the future, however the reason why we are developing websites are for our users, and some of them are still in the past (ie9 ahaha), that's why it's still needed to know Float as fallbacks, better Table, for these two CSS layouts.
https://www.smashingmagazine.com/2017/07/enhancing-css-layout-floats-flexbox-grid/

	nah, just realized that Grid is just like a more specific Table having x,y components. So no need to learn Table. Also learned that "inline-block" is much better fallback than "float". Feature queries will really help. Susy as fallback too will help
	https://www.chenhuijing.com/blog/basic-grid-with-fallbacks/#altogether-now

	learn Susy2!
  ```

**Thoughts** I really thought I could finish this project today, I'm now delayed big time, this is just my first ever FCC project. But, I also realized that the next four Responsive Web Design will not really challenge with respect to layout-ing, except the portfolio. What I mean is that, I'm grateful that I'm learning this now, I'm learning alot. I also realized how useful the workflow or shall I say studyflow of "solve problem" -> "can't solve on own" -> "watch tutorials" VS. the typical Watch all tutorials then solve problems/build projects. Wuhooo!
![r1d4 screenshot](https://github.com/jbbalderas/100-days-of-code/blob/master/intl/r1d4%20screenshot.png "Look at 'em CSS. Tried so many things, haha")

**Link(s) to work** [Tribute Page deployed online](https://jim-rohn.netlify.com/)

### Day 5: July 11, Wednesday

**Today's Progress**:

```
11.19a
	Decided to learn the basics first then continue.

	re: positioning/layout concern before flex & grid: https://learn.shayhowe.com/html-css/positioning-content/

		try layout using tables->divs->flex https://forum.freecodecamp.org/t/i-do-not-like-css/107908/40?u=jbbalderas

		a good video series of CSS resiliency and relationship w/ 'The Web' formation https://hacks.mozilla.org/2018/03/how-to-write-css-that-works-in-every-browser-even-the-old-ones/

		a great CSS trick for centering vertically and horizontally 	https://forum.freecodecamp.org/t/the-greatest-css-layout-trick-youve-ever-learned/64451/2?u=jbbalderas
			position: absolute;
			left: 50%;
			top: 50%;
			transform: translate(-50%, -50%);

		box-sizing: border-box 		greatest CSS trick 		https://forum.freecodecamp.org/t/the-greatest-css-layout-trick-youve-ever-learned/64451
			also {height:100vh} and {min-height:100vh}
			also re: centering w/ flex 		{ display: flex; justify-content: center; align-items: center; }
			also calc() 	ex:width: calc(20vw+50px) 	calc: (100vh - 10px); when you want 100vh but have some other pesky element messing it up such as a menu or footer
			also "inline-block + box-sizing: border-box" eliminates need for floats though needs to redeclare the font-size as (width+font-size) is how inline-block calc

	an FCC moderator with leader as trust level answered the question: 'Should I fully learn how to use HTML & CSS before using a framework like Bootstrap?'
		No. You should get to learning how to program, and then circle back to HTML and CSS. ...When you build projects, you’ll find yourself learning all the CSS and HTML you need.
		https://forum.freecodecamp.org/t/i-have-hit-a-wall-with-my-learning-progression-and-i-need-help/84878/3?u=jbbalderas
		https://forum.freecodecamp.org/u/PortableStick
		WOAH
	This workflow may help:

		Plan basic layout and/or functionalities on a piece of paper (or your tablet)—don’t go overboard and plan every little thing because it’s a waste of time, your might as well start coding if you are writing down the logic of a form submission
		Create the skeleton of your page with <div>s (or any other appropriate elements of your choosing), make sure that everythingis positioned as you intend them to be
		Be as diligent and sensible as possible with applying classes your <div>s—it will save your time once you want to start stylising things
		Use box-sizing: border-box; and border: 1px dashed black; to visualise your <div>s as necessary
		Let the page be ugly
		Really, just let it be ugly for now
		Put text and pictures in and make sure everything is positioned properly
		Style things and check again that things are working properly
		Show people when it’s done (you may not get feedbacks sometimes because not everyone has the time to do it—in cases like that, show your family and friends)
		https://forum.freecodecamp.org/t/i-dont-feel-right-doing-this/151446/3?u=jbbalderas

Realized that I need to learn Flex then Grid, but also consider the fallbacks using Feature Queries. Question is, w/c is best or most used? (table; inline-block; float; susy)

	Display: Inline 	ignores width, height and vertical margins/padding 			THUS, display: inline-block
		1] Inline, 2] Block, 3] Inline-block, 4] float: left/right + clearfix, 5] display:table, 6] position:relative, 7] position: absolute, 8] z-index: [#]
		https://medium.com/@amykurtz04/top-8-css-values-i-wish-id-understood-earlier-1879f9daca75

	1] Tables for centering, 2] Justify Grid for IE6+, 3] IE6+ w/o box-sizing:border-box, 4] color property is inherited https://www.silbinarywolf.com.au/post/132256749898/4-things-i-wish-i-knew-about-css-a-year-ago

1.40p Decided to go back to tutorials for Layout and Positioning. Recently browse resources I have and realized there's a lot to be learned and I'm glad

	Stanford's CS193c -> colt's WDBC -> rob's TCWD2 -> Todd's HtCaW:aHTaCT -> ShayHowe positioning -> FCC curriculum


4.20p
	Stanford's CS193c day 3
		Microformats
		< data- >
		Float layout if you wanna work for old companies, ex: new york times. The teacher, Dr. Patrick Young actually has a handout for this bc he hasn't found any good recommendable resource online compared to flex & grid.
			clear: both (left & right) 		-> nothing to float on my left or right 		VS 	overflow: hidden

		Flexbox is not designed to layout web pages; It should be used in conjunction with Grid. 1D layouting only.
			flex-direction| order| flex: wrap/nowrap| justify-content| align-items| flex-grow| 

		Grid

		<Article> can have at most 1 H1. Rule: one H1 per HTML		
			fr = fraction| explicit vs implicit grid| repeat| minmax| grid-auto-columns/rows vs grid-template-columns/rows| grid-column/row-gap| grid-column/row-start/end| 
	Susy - Don't use my grid
		Chapter 3: 
			First step: Fix the Box Model 	*{box-sizing: border-box}
			2] Avoid Tightly Coupled elements
			3] Whenever you can... go with The Flow

		Chapter 4: Layout techniques [pre 2017]
			-👎relative positioning | absolute positioning 		Only good for overlays (off-canvas, drop-downs, tooltips, modals, etc..)
			-CSS Floats 	+ Micro clearfix 	.clearfic::after{ clear: both; content: ''; display: table;} 		+ display:flow-root Ahaha
				 -overflow:hidden 		(hack) for 'fluid containers', and 'clearing containers'
				 -👍floats are greate for Flexible Markup & Nesting
				 -👎always 'Define the Width'
			-Sub-Pixel Rounding 		(sub-pixel floating > sub-pixel isolation)
			-👎Inline-Block
				mainly used for vertical centering (invasive and confusing hacks required)
			-Display: Table? 		(no margins, use border-padding) 		display: table/table-cell

			-👍 Flexbox 	 	(kinda like floats+display-table, but 'not a hack')
				-👍Flexing is 'Magic' 		play with these relationships 	flex-grow/shrink/basis
				Flex-basis defaults to width (w/c defaults to auto)
				-👎Still a One-Dimensional Flow 	(w/ line-wrapping soln's)
				-👎Nesting matters too much 	(we need "display:contents")
				-👎Poor performance for Page Layouts	
					loads slowly
		Chapter 5: Grid Systems, A Historic Detour
			👍Provides Consistency
			👎Enforces Consistency
				Bootstrap projects all look the same, and that's boring
			👍Shared CSS Hacks
			2007 Blueprint CSS - first ever Open Sourced CSS
				Classes are the API -> Clear APIs are good -> Developers can ignore CSS -> -> Developers ignore CSS
				Best for Massiv Codebase over long periods, w/ too many devs, and little communication NOT for small agency trying to design unique things
			2009: Object Oriented CSS
			2010: 960 grids
			2008: Natalie Downe talk at Barcamp London 5 "CSS Systems"
				idea: create consistent ways of building websites instead of creating tools that would make us do exactly the same time
			Consistent Systems, Custom Grids
				Frameworks Lock You In, fine until you try something new...

			Grid built w/ percentages 	(container defined with ems/max-width: 100%)
				👍container responds to Viewport and Font-size (contents respond to container)
				👍no restrictions
				👍no ugly classes
				👎ugly math & meaningless numbers...
			Susy 	(patterns add meaning)
			Responsive Web Design ™		(fluid layouts, w/ fluid images, and media queries)
				Mobile First 	(design for the smallest screens, then build up)
					@media(min-width: 35em){/* larger layout...*/}

			👍Any Grid System, On Demand (just pass in different settings...)
			👎Grid Systems are overkill

			Bootstrap - tiny bootstraps for every client

		Chapter 6: DIY Grids 	(with any layout techniques)
			How you avoid using grid systems now
			Fluid grids require math 	(make the math simpler)
				target/context == multiplier
					width: percentage(target / context)

			Margin Gutters ruin the math
				Span 3 of 12 [w/o gutters]
				//float, or flexbox, or css-table... 	.element{width: percentage(3/12);} 	|| .element{width:calc(3/12 * 100%)}

				Like CSS Systems for OOCSS 	(simple math, open system)
					using fractions, doing it on the fly

				👍No ugly classes
				👍Works with any technique
				👎Implicit relationships > Explixit grids 	(let the browser figure it out...)
					there's no magic in grids, not a design savior.
		Chapter 7: Paradigm Shift 	(CSS becoming more extensible)

	Okay, at this point, I realized what if the slides are available online? 	Bengga https://oddbooksapp.com/book/djangocon-layout

			Calc + Custom Properties == Grids! 	(media queries can change settings)				

			Vieport Units (vw,vh,vmin,vmax) 	gives us some more control

				Full-height... 	height: 100vh 	(remember to set overflow)

		C. 8: CSS Grid 	(omg, why did we talk about anything else?)
			if you can start using Grid, start using Grid!
			FR defines a fraction of remaining space

		gridbyexample.com 		(usable templates with fallbacks already written...)

		Susy3 is a Fallback Plan 	(grid-like functional syntax)

		C.10: Just do it
			Start w/ the grid
			Fix the Box Model
			Stay in the Flow
			Think Dynamically (how do objects relate and change?)
			Remove External Gutter Math
			Get Creative! 	(the world is ready for more than 12 columns...)

		Wow. Just great find. I'm glad I found this article https://css-tricks.com/dont-use-grid-system-others/
			It's so interesting that the founder of Susy is now calling us to NOT us her grid system
			https://2017.djangocon.us/talks/don-t-use-my-grid-system-or-any-others/

	CSS Grid Changes EVERYTHING - Amazing Presentation
		CSS Grid: A Practical Approach for Today
			1. Build accessible mobile-first layout w/o grid
			2. Use mobile-first layout as fallback for all brosers.
			3. Use #supports to detect grid support
			4. At the appropriate breakpoint, create layout with grid and grid-areas
			5. Explore new layouts as viewport widens
		Your path to CSS Grid
			Firefox has a grid inspector 	https://goo.gl/SJmlms
			gridbyexample.com
			MDN has exhaustive documentation
			CSS Tricks has a Complete Guide to CSS Grid
			Kuhn
			Building Production-ready css grid layouts today 		goo.gl/dae838
		1. Make it accessible
		2. Make it fancy
		3. Make sure the fancy doesn't break the accessibility
			mor10.com/wceu2017
  ```

**Thoughts** Yesterday, I was so eager to learn or master at least one fallback for flex and grid. But after studying today, I realized that Grid is the future, as well as Grid is the now! Fallbacks via feature queries are available and there are resources available online for this. I'll still go through all the available resources (tutorials and exercises) I have now, and it's just encouraging to know the CSS evolution or just 'the timeline' on why there's so many hacks or different ways available to layout, then ultimately there's CSS Grid as the ultimate destination (for now). However, I also learned that I need to get to JavaScript programming as early as possible and learn the basics of HTML CSS, for I can see that in the future, the laying out or positioning of websites can be done by AI by just giving them the design. Yeah I know, they can do this things, but the creativity and imagination is still on us, AI's can implement but the complexity of creativity to solve variety of problems (not just one) is still on us. Construction and designing of a building/house/shop can be automated in the future, but the furnitures inside and the functionalities as to why people are going inside are still being decided by us.

**Link(s) to work** 
1. [Shay Howes CSS Positioning Contents](https://learn.shayhowe.com/html-css/positioning-content/)
2. [CSS Resiliency Video Series](https://hacks.mozilla.org/2018/03/how-to-write-css-that-works-in-every-browser-even-the-old-ones/)

### Day 6: July 12, Thursday

**Today's Progress**: 

```
11.20a Continue studying

	15 reasons why a grid based aproach will improve your designs
		1. Organized Content
		2. Quicker job
		3. Aligned typoraphy
		4. Easier to Collab w/ 
		5. Easier Balancing of design
		6. MultiPage Layout Cohesivity
		7. Visual Hierarchy can be enhanced
		8. No Cluttered layouts due to margins and gutters
		9. Math based pleasing designs. ie: rule of thirds
		10. Extra Impact when breaking grid
		11. Highly Flexible
		12. Can help you go diagonal
		13. Any medium of design
		14. Can encourage white space
		15. More digestible and readable for viewers

		https://www.canva.com/learn/grid-design/
1.40p CS 193c day 4
	Positioning 	(good for advertisements)
		absolute, fixed, relative
		'relative' leaves a space while 'absolute' doesn't
	
		iFrames (can be used as an article inside webpage; A different/separate html file; not to be used these days. )
	Responsive design
		usually server side decision w/c stylesheet to give
		printer? mobile? desktop?
			<link rel="stylesheet" href="" media="print">
	Media Queries
		now it's what properties their device have
			<link rel="stylesheet" href="" media="screen and (max-device-width: 480px)">
			or <style>@media(min-width:480px){h1:18pt;}</style>
					  @media screen and (orientation: portrait){#nav{display:none}}
		Standards remnant from attempt to include JavaScript on CSS
			calc 	for (+,-,*,/) always use space between them operators

			Custom Properties 	(CSS Variables)
				:root{ --myVariable: 50px; } 
				to address example 	| margin: var(--myVariable);
	55:11 to 1:32:00 	all about Forms
	1:32:00 onwards
	alternative to sprites = Image Map 		
		(clicking to specific parts of an image will direct to another link/page | anchor tags via coordinates area on image)
	character entities
		&amp; for ampersand, since "&" means a break

	FTP (way to upload your website files to your ISP/Server provider)
		ex: secureCRT 		just like Filezilla or Putty

	Don't use capital letters and space on filenames

✓Stanford's CS193c -> colt's WDBC -> rob's TCWD2 -> Todd's HtCaW:aHTaCT -> ShayHowe positioning -> MDN CSS Layout -> FCC curriculum
 
4.30p Decided that before continuing to WDBC, since I have skipped the assignment parts of the previous concepts taught, I'll finish them first because that's what I need, the exercises.

4.55p Scanning my external HDD let me find a Sublime Text 3 screencasts from codeschool. :D cool 8min watch
	ctrl K+B sidebar
	ctrl L 					select all line of current selected
	ctrl K 					remove line at a time
	ctrl shift P + "re"		reindent lines :O
	ctrl 	[ or ]	 		manual indent left or right

	ctrl shift G 			Emmet wrap (for wrappers ex: div or anchor tags) 	cool
	ctrl shift L 			breaks each line selection's into independent selection 		usually combined w/ Emmet Wrap

WDBC
	exercises: HTML recreate website , CSS Selector
	em 			Relative to parent's font size 			double the size = 2.0em
	100-800 	font-weight values 			light - heavy

	exercise: CSS blog from scratch
		Things I missed and learned:
			border-left
			REM 			not by parent element, but by Root
			hr styles available online :D

  ```

**Thoughts** I decided to power through all the necessary fundamentals or all the related topics or concepts that's available on all of my resources. So far my progress is somehow slow because I think I have wasted alot of time today (those extended breaks), but still I commend myself today. Although, I also know that there's so much more left to study, so better maximize the time alloted tomorrow. Way back before on my internship, I also tried to study (I mean watch) all the tutorials but dreaded all the exercises or assignments provided. Now it's the opposite, I decided to power through all the assignments for better learning. Knowing bits of learning how to learn really helps. Today I feel determined to continue. #deliberatePractice

**Link(s) to work** Same as day 5

### Day 7: July 13, Friday

**Today's Progress**: 

```
1.56p Study
	Rob's TCWDC2
		position: relative; + left/right: -50px; 	+ 	z-index:; 	+ 	opacity: 0-1;
		position: absolute is just like 'in front of text' or 'behind text' on MS Word (out of the flow)

		column-count; column-gap; column-rule-style; column-rule-width; column-rule-color;

5.26p Todd's HtCaW:aHTaCT
		main.css as convention
		client-side: Node>django>ror 		|| server-side: go >>> PHP, ASP, CFM
		css, js, img, pic 		folder structure convention

		background-size: cover; 	+ bacground-repeat: no-repeat 	for imgs
		Rendering engines

		good document structure's why: maintainability, readability, accessibility, search engine rank
		Document Object Model (DOM)

	http://learnlayout.com/
  ```

**Thoughts** I'm ending this day in an excited state coming from a sleepy state at the start. Why? I started studying at 1:56 pm today after having an almost three hour basketball (shooting drills + 21 + horse + 11 + 1v1) in the morning while having an intermittent fast (my first meal's at 2:30pm). Ahaha. I know, but I powered through Rob's teachings, ate lunch then read "The Magic of Thinking Big" for 30 min, then got back to Rob's eventually finishin what I need. Then I jumped on Todd's and after watching my last video for the day of which an overview of CSS layout (w/c is the main reason why I came back to tutorials to finish my tribute page), I got excited for tomorrow because of partly my why but mostly his teaching style. Todd always zoom out to the forest every after looking on each tree, I also like his motivation from time to time relating to craftsmanship and Web Dev as also an engineering discipline. #Funda

**Link(s) to work** Same as day 5 + http://learnlayout.com/

### Day 8: July 14, Saturday

**Today's Progress**:

```
11.19a Continue Studying
✓Stanford's CS193c -> ✓colt's WDBC -> ✓rob's TCWD2 -> ~Todd's HtCaW:aHTaCT -> ShayHowe positioning -> MDN CSS Layout -> FCC curriculum

Todd's
	font:
		font property: (== font-style + font-variant + font-weight + font-size + line-height + font-family)

		serif has feet. Sans serif, most preferred on web, doesn't have. Sans = none/without. Serif = slight projection of a finished stroke

		font-size: vw > rem > px 		(viewport width > Root M (default font size) > pixels) 
			common size-ing usage
				% : 	width & height of 	containers, divs, and responsive imgs
					https://medium.com/@madhum86/css-font-sizing-pixels-vs-em-vs-rem-vs-percent-vs-viewport-units-b1485716afe7
				*fluid responsive > adaptive (vw > media queries + rem) 
					https://www.elegantthemes.com/blog/divi-resources/better-mobile-website-design-how-to-use-vw-vh-and-rem-to-create-fluid-divi-pages
		external font first before external css
		"always monitor the weight of everything you're downloading (weight = file size) via Dev Tools>network"
		Ctrl + Shift + R 	== hard refresh
	Display
		</nav><!-- you can't leave a space or return her --><main>  	an HTML bug/quirk/feature 		having display:inline-block
1.48p http://learnlayout.com
	'position: absolute' behaves like 'position: fixed' but relative to the nearest positioned ancestor, NOT the viewport.

	'display: inline-block' layout
		elements are affected by the 'vertical-align' property, w/c you probably want set to top
		theere will be a gap between the columns if there is any whitespace between them in the HTML
	column-count 		as answer to prevent annoyance when reading long lines of text

	flexbox centering 		'align-items: center' + 'justify-content: center'
2.20p done w/ learnlayout.com

5.30p Decided to call it a day, since it's Saturday and I got appointment from 6pm to 11pm

✓Stanford's CS193c -> ✓colt's WDBC -> ✓rob's TCWD2 -> ~Todd's HtCaW:aHTaCT -> ✓learnlayout.com -> ShayHowe positioning -> MDN CSS Layout -> FCC curriculum

Things to do:
	☐	optimize those two small img for the tribute page 
   ```
**Thoughts** Way way more to go. I was thinking if right now, my strategy of learning is right or it can be improved. I just wonder if it's right to pick only one project from FCC RWD projects then study the necessary and relevant materials needed. Or I should study all the materials and every time I end a concept or knowledge, I should try to implement it in a project, thus, I will work on the five projects simultaneously. But as I'm typing this, I also realized that the latter part can be good to minimize time for learning and accomplishment of projects, but the workflow for each project will not be realistic in terms of what happens in real dev work wherein you just focus on one or two projects, design then build, then as you encounter holes in knowledge, you research and study how. So as of this writing, I'll stick with the first option. Besides, I feel great with what I'm learning for I know I'm gaining traction little by little to my dreams of creating helpful things out of nothing. :) #GoodFoundationFirst 

**Link(s) to work** same as day 5


### Day 9: July 15, Sunday

**Today's Progress**: Zoom out on coding and learn things related to it.

```
5.13p Googled: "mistake" "full stack developer" "web"
	It’s tempting to dive straight into Javascript or Python because it might seem more interesting, but ultimately that would be a mistake. (re: Step 1 – Learn HTML)
		http://fullbit.ca/2018-full-stack-developer-road-map-part-1-front-end-development/

	"mistake" "wish" "realized" "taught" "learned"
	• Having to clean up old code mistakes is a lot more time-consuming than planning thoroughly and doing things right from the start.
	• a mistake I think many rookies make is to consider a computer science degree a substitute to self-learning or a bootcamp, as a means of becoming a web and/or mobile developer. Based on my experiences, this is not accurate.
	• On a final note, a mistake I think many rookies make is to consider a computer science degree a substitute to self-learning or a bootcamp, as a means of becoming a web and/or mobile developer. Based on my experiences, this is not accurate.
	and it taught me an important lesson. In the world of Agile software development, lone wolfing isn’t an option. Teamwork is a major part of finding a productive workflow. (re: not reaching a productive level in line w/ the rest of his team)
		https://medium.freecodecamp.org/how-i-landed-a-full-stack-developer-job-without-a-tech-degree-or-work-experience-6add97be2051

	• The most common mistake in web design is being inspired by web design. It’s easy to get in a loop of looking for inspiration in the kind of things we’re already making. -Jessie White, Associate Creative Director, Instrument

	• One of the most common mistakes I see is having text and elements too close to each other. When things are visually messy, it makes users want to leave your site sooner. -Wes Bos , Full Stack Developer and Teacher of all things web

	• One mistake I seem to catch again and again is the overzealous use of the overflow property in CSS, specifically ‘overflow: scroll.’ -Skylar Challand, Founder, Oak

	• Once the creative process has kicked off, a common mistake I see interactive designers make is separating the design phase from the technology phase. It’s easy to layout some great looking static pages in Photoshop or Sketch, hand over the files to a developer, and move on. But exploring the technology angle simultaneously with the creative approach is what sets great websites apart from average ones. -Melissa Showalter, Art Director, Instrument

	• I think the most common web design mistake I see is sites not respecting users and their time. (Bloated, slow-loading pages; Overly-aggressive advertising; Popups and overlays; Dark patterns; Other superfluous or intentionally deceptive practices I lovingly classify as bullshit.) -Brad Frost, author of Atomic Design

	• A mistake I often see designers make is treating web design like print design... Unlike print, which is static and can be tightly controlled, great web design must be based on a super flexible, highly considered system that addresses all the crazy use cases that come with the modern internet. -Patrick Richardson, Co-Founder, Executive Director, Franklyn

	• The most common Web Design mistake I see is lack of compelling content. -commenter Michelle Hickey

	• so many major e-commerce sites not calling the correct mobile keyboard for specific form fields or overlooking the autocorrect, autocapitalize and autocomplete attributes for mobile forms. Unfortunately, that seems to be the case with the name and email inputs of this form as well. -commenter Adam Lane

		https://blogs.adobe.com/creativecloud/experts-weigh-in-what-is-the-most-common-web-design-mistake-you-see/

	• The secret is to learn ONLY ONE THING at a time.
		https://ihatetomatoes.net/3-steps-becoming-better-front-end-developer/

Jay Shetty's Strengths Finder
	1. Uncover your strengths
		16personalities.com
		1.1 Ask at least three persons, as detailed as possible your skills, expertise, talents
		1.2 Find patterns
		1.3 Writing your own job description based on what people said, and the themes and patterns that you see, and how you see your self.
	2. Becoming an expert (invest in your strengths!)
		2.1 read books
		2.2 networking (shadow, volunteer, intern)
		2.3 online course
		2.4 start an MVT minimum viable test
	3. Living and breathing your strengths (apply!)
		volunteer, workplace, 

		via Email subscription
https://edgecoders.com/the-mistakes-i-made-as-a-beginner-programmer-ac8b3e54c312
	1) Writing code w/o planning
		Do not think about programming as writing lines of code. Programming is a logic-based creativity that needs nurturing.
	2) Planning too much before writing code
		Planning all the features at once should simply be outlawed!
	3) Underestimating the Importance of Code Quality
		use ESLint and Prettier
		-Using many lines in a function or a file
		-Using double negatives. Please do not not not do that.
		-Using short, generic, or type-based variable names. Give your variables descriptive and non-ambiguous names.
		-Hard-coding primitive strings and numbers without descriptions.
		-Using sloppy shortcuts and workarounds to avoid spending more time around simple problems. Do not dance around problems. Face your realities.
		-Thinking that longer code is better.
	4) Picking the First Solution
		find the simplest solution to the problem. By “simple” I mean the solution has to work correctly and perform adequately but still be simple enough to read, understand, and maintain.
	5) Not Quitting
		sticking with the first solution even after I identify that it might not be the simplest approach. when it comes to writing programs, the right mentality is fail early and fail often.
	6) Not Googling
	7) Not Using Encapsulation
		If you make a simple change and then discover that the change has a cascading effect and you need to do many changes elsewhere, that is another sign of newbie code.
		Have High Cohesion and Low Coupling, which is just a fancy term that means keep related code together (in a class) and reduce the dependencies between different classes.
		This is not about secrecy but rather about the concept of reducing dependencies between the differenet parts of an application.
	8) Planning for the Unknown
		Always write the minimum amount of code that you need today for the solution that you are implementing. Handle edge-cases, sure, but do not add edge-features.
	9) Not Using the Right Data Structures
		to manage a LIST of records you should use a MAP.
		just use a Stack structure. it is usually hard to optimize recursive code, especially in single-threaded environments.
	10) Making Existing Code Worse
		Duplicating code.
		Not using configuration files.
		Using unnecessary conditional statements and temporary variables. 
	11) Writing Comments About the Obvious Things
		Most comments can be replaced with better-named elements in your code.
	12) Not Writing Tests 
		Testing-driven development (TDD) is not just some fancy hype. It positively affects the way you think about your features and how to come up with a better design for them.
	13) Assuming That If Things are Working then Things are Right
		handling of invalid input
		 handling for empty input.
	14) Not Questioning Existing Code
		As a beginner, you should just assume that any undocumented code that you do not understand is a candidate for being bad. Question it. Ask about it. git blame it!
	15) Obsessing About Best Practices
		There are no best practices. There are probably good practices today and for this programming language.
	16) Obsessing About Performance
		Premature optimization is the root of all evil (or at least most of it) in programming — Donald Knuth (1974)
	17) Not Targeting the End-user Experience
	18) Not Picking the Right Tool for the Job
	19) Not Understanding that Code Problems Will Cause Data Problems 
		Use multiple layers of data integrity validations. Do not rely on the single user interface. Create validations on front-ends, back-ends, network communications, and databases. If that is not an option, then you have to at-least use database-level constraints.
		If multiple operations need to change the same data source and they depend on each other, they HAVE to be wrapped in a transaction that can be rolled back when one of these operations fail.
	20) Reinventing the Wheel
	21) Having the Wrong Attitude Towards Code Reviews  
	22) Not Using Source Control
	23) Over-Using Shared State
		The big problem with shared state starts to happen when multiple resources need to change that state together in the same tick of the event loop (in event-loop-based environments). Race conditions will happen.
		A newbie might be tempted to use a timer as a workaround for this shared state race condition problem, especially if they have to deal with a data lock issue. That is a big red flag.
	24) Having the Wrong Attitude About Errors
	25) Not Taking Breaks

https://medium.com/the-mission/most-people-think-this-is-a-smart-habit-but-its-actually-brain-damaging-9a6f3d6bccc9
	• Junk Learning Source #1. The “Facts” We Know Are Slowly Being Debunked
		Learning physically changes our brain.
		Much of the learning that people are exposed to by default is junk learning.
		Junk learning effectively equivalent to brain damage and impairs our ability to function in the world.
		Junk learning is like a disease that spreads throughout the brain and causes more junk learning.

	Lesson Learned: Look for information that actually increases in value over time. When it comes to knowledge, think like an investor, not a consumer.

	• Junk Learning Source #2: A Little Knowledge Is Dangerous
		Dunning-Kruger effect: least knowledge == highest confidence; 
	Lesson Learned: No matter how much we know, we only know a fraction of all there is to know. We must assume our own ignorance. An attitude of caution can help us avoid developing false beliefs that can lead to irrational decisions.

	• Junk Learning Source #3: Our Confirmation Bias Makes Us Progressively More Dumb
		One of the biggest daily examples of confirmation bias involves our social media bubbles: We read the same sites, listen to the same friends (who agree with us!), and watch the same news over and over, which only confirms what we already believe. When we’re exposed to something that doesn’t fit our model of the world, we unconsciously either ignore it, minimize it, or attack it

		We learn the most by proving ourselves wrong, not by proving ourselves right. Many of the greatest thinkers of the 20th century independently came to this conclusion.
	Lesson Learned: We need to identify and stress-test our most fundamental beliefs about the nature of reality — and learn how to handle the strong emotions that will come up when we do.

	• Junk Learning Source #4. We Trust the Wrong Ideas and the Wrong People
		Halo Effect: a cognitive bias that makes us trust a person’s advice in one area of life simply because they are an expert in another area.

	Lesson Learned: As a result of reading The Halo Effect, I’ve become much more suspicious of listening to celebrity experts in any field. Instead, now whenever I look at who to emulate, I specifically look for people who have experienced success over and over not because of luck or celebrity, but because of skill. In my experience, many of these individuals are not celebrities. Then, I carefully experiment with their advice to see if it will transfer to my context.

	• Junk Learning Source #5. Over-specialization limits our ability to learn across disciplines
		keeping in mind that it is difficult to predict what skills will be required two or three decades from now, the best option seems to supplement the teaching of specific knowledge with the teaching of metaheuristics that are transferable (Grotzer & Perkins, 2000; Simon, 1980). These may include strategies about HOW TO LEARN, HOW TO DIRECT ONE’S ATTENTION IN NOVEL DOMAINS, and how to monitor and regulate one’s limited resources, such as small STM [short-term memory] capacity and slow learning rates.

	Lesson Learned: Being too specialized can hurt future learning if done alone. Supplement by spending more of your time learning fundamental knowledge that doesn’t change. This is why we created the Mental Model Club.

	[Take Action: Strengthen Your Brain Instead of Damaging It]
		learning how NOT to learn can help us learn faster and better

		1. Our “facts” are expiring and we don’t even know it.
			When it comes to knowledge, think like an investor, not a consumer.
		2. A little knowledge is dangerous.
			Realize you only know a little bit.
		3. Our confirmation bias makes us progressively more dumb.
			Identify and stress-test your most fundamental beliefs
		4. We too often trust the wrong ideas and the wrong people.
			Be super careful about whom and what you choose to emulate.
		5. Over-specialization limits our ability to learn across disciplines
			Instead, spend most of your time learning fundamental knowledge that doesn’t change such as mental models.
   ```

**Thoughts** On a Sunday, I defaulted to considering this as a rest day from coding. But I've got free time today, so I tried to Google questions in my mind. I also tried to star some email addresses on my primary email (so that none of them will go to spam), then tried to backread on what I missed and I'm satisfied to what I learned regarding typical mistakes of becoming a programmer/developer. I also got another chance to know more of my strengths, even though I already took the strengthsfinder 2.0 test online. Lastly, I learned how 'mental models' and 'principles' are the necessary foundations for our brain and of course in living a good life. #fundamentalsLast

**Link(s) to work** none

### Day 10: July 16, Monday

**Today's Progress**:

```
10.59a

https://medium.freecodecamp.org/mistakes-i-have-made-as-a-junior-developer-85260bdb992f

https://medium.com/the-mission/2-eye-opening-experiences-that-trigger-immediate-clarity-and-behavior-change-7ad42561db6
	1. Seeing someone else operate w/o fear (frontliners)
	2. Have someone you love/respect tell it to you straight (feedback)

https://hackernoon.com/how-not-to-be-a-mediocre-developer-c59a49f97fc5
	write more code
	incorporate tests
	be hionest
	contribute to open source
	be open to help
	pick a personal project
	lower your ego
	understand the 'why'
	don't be lazy
	solve coding challenges
	encourage the good stuff
	don't hid behind the layer
Web Architecture 101
	1. DNS
	2. Load Balancer
	3. Web App Servers
	4. DB Servers
	5. Caching Service
	6. Job Queue & Servers
	7. Full-text Search Service
	8. Services
	9. Data
	10. Cloud Storage
	11. CDN
   ```

**Thoughts** Trying to look to larger pictures and helpful articles for this journey. (Again) since I scheduled this day to meet an old friend (High School best friend), but she forgot about it. I'm writing this thought on day 11, Tuesday, since I got derailed by what happened yesterday. I think now I'm aware that hurdles or obstacles like that one where I felt disappointed must be acted with self-awareness. I must be aware that I'm feeling that emotion, and act to snap out of it so that I can continue having 'traction' pursuing my dreams instead of 'distraction'. #thoughtsFired

**Link(s) to work** same as day 5
   
### Day 11: July 17, Tuesday

**Today's Progress**:

```
1.37p Finish Todd's

Layout Essentials 	goo.gl/k7hbXq
	Chapter 17. Layout with Position
		position: fixed
			nav, footer, modal
		position: relative
			- "relative to itself"
			- element's original space in the DOM is still blocked out
		position: absolute
			- "in relationship to the next element UP the DOM, that also has position set than the default - static"
	Chapter 18. Layout with Float
		wrap around an image
		-element should be 'taken from the normal flow' and placed along the 'left or right side of its "container"',
		where '"text" and "inline" elements will wrap around it'

		-overflow 		happens when the container is smaller than the floated element
			fix 		overflow: auto
		-clear: left/right/both
	Font boosting
		history: done by mobile browser. Randomly increase font sizes. Ex: two long Lorem paragraphs, but no boosting if just one
			hacky sol'n: 	p{max-height: 1000000px; -webkit-text-size-adjust: 100%; -ms-text-size-adjust: none;}

		meta-viewport tag
			RULE: ALWAYS INCLUDE
		<meta name="viewport" content="width=device-width, initial-scale=1">
		width=device-width 		make the html/body's width = device-width
		initial-scale=1			mapping CSS pixels to 'device independent pixels' (physical pixels = hardware pixel)

		font boosting isn't needed if meta-vieport tag exists

✓Stanford's CS193c -> ✓colt's WDBC -> ✓rob's TCWD2 -> ✓Todd's HtCaW:aHTaCT -> ShayHowe positioning -> MDN CSS Layout -> ~FCC curriculum

Study Fundamentals
- Finished Todd's HtCaW:aHTaCT that's relevant to layout and positioning.
- Did 30 min. of FCC's exercises.
   ```

**Thoughts** I haven't maximized my typical study time of 6 hours, today I just studied for 3 hours. I can see that it's because my morning routine got derailed by one big chunk and I guess it's one of the keystone habit that I've established these past two weeks. Failure again, so here I am, writing that next time, if I missed a habit (keystone or not) I should think of an alternative similar task or just commit to do the next habit/task/routine in queue at the proper time. #MistakeAdmitCorrectLearn

**Link(s) to work** same as day 5


### Day 12: July 18, Wednesday

**Today's Progress**:

```
1:08p FCC curriculum challenges

✓Stanford's CS193c -> ✓colt's WDBC -> ✓rob's TCWD2 -> ✓Todd's HtCaW:aHTaCT -> ShayHowe positioning -> MDN CSS Layout -> ~FCC curriculum

"Accessibility" generally means having web content and a user interface that can be understood, navigated, and interacted with by a broad audience. 
	Some users rely on assistive technology such as a screen reader, voice recognition software, keyboard
	1. have well0roganized code that uses appropriate markup
	2. ensure text alternatives exist for non-text and visual content
	3. create an easily-navigated page that's keyboard-friendly

	WCAG W3 Consortium's Web Content Accessibility Guidelines

alt attrib 		= describes content of image & provides a text-alternative (img failed to load). Used by search engines.
				good alt text is short but descriptive, and meant to briefly convey the meaning of the image.
				MANDATORY required per HTML5 spec
					unnecessary if 1] img is group with a caption, 2] used for decoration only ex: bg image
				Note: imgs w/ a caption, including ALT text helps search engines catalog the content of the image.

5.03p enough with FCC, start rob's TCWDC2 hands on exercise of "clone BBC News Website"

meta:vp


"always try to work from the innermost element, style that, and make that work, instead of styling multiple outer elements" 
	-jesse showalter https://youtu.be/Boc_IZNzlh4?t=14m55s

   ```

**Thoughts** Today I got humbled by this experience of trying to clone BBC news website. I struggled to quickly recreate the reference site's first navigation bar out of three just by using floats and positions. Halfway of my studying time today, I'm still struggling with vertical alignment of the navigation buttons so I took a break, got some light sweat, cleared that brain fog, then came back. I remembered Jesse Showalter's particular vid on his 'code and design' playlist where he is building his nav bar also. And so I watched it again and boom, one of his tip struck me, as I rewind for 10 seconds he said "always try to work from the inner most element, style that, and make that work, instead of styling multiple outer elements". There I rebuilt my CSS from the the innermost <a> elements for the vertical alignment and filling of the box model, and boom! I still am proud of what I've done and progressed today. #moreExperiencesPlease #danceWithFear

**Link(s) to work** [clone BBC news website](http://completewebdevelopercourse.com/clone/)


### Day 13: July 19, Thursday

**Today's Progress**:

```
12.04p

best practice to set box-sizing to border-box
	*, *:before, *:after {
		border: 1px dashed green;
		box-sizing: border-box;	
	}

	https://internetingishard.com/html-and-css/css-box-model/

https://www.quora.com/What-are-some-good-practices-to-organize-CSS-code
	-Use comments where you think there are needed. Don’t comment what the CSS codes do but why you wrote that CSS.
	-The best way/time to organize CSS code is when you are writing your stylesheet. 
	-Put all CSS codes that are general to the page like typography, miscellaneous/`general trick` on top of the page.
	-Write your CSS code flow (top to bottom) accordingly to your HTML code. Use comment to delimit different section of your CSS code.
	-Write the CSS properties for selection in alphabetical order.
	-Use proper name and convention for your selector. `block-left` and `block-right` is better that `b1` and `b2`.
	-Organized your asset folders (images)
		CSS Naming Conventions that Will Save You Hours of Debugging
			-Use Hyphen Delimited Strings
			-The BEM Naming Convention
				--why?
					1] Know what it does
					2] Idea where it can be used
					3] Know relationships bet. class names
				B = Block
					.stick-man
				E = Element/s 			(two underscores)
					.stick-man__head
					.stick-man__arms
				M = Modifiers 			(two hypens)
					.stick-man__head--small
					.stick-man__head--big
			"There are only two hard problems in Computer Science: cache invalidation and naming things" — Phil Karlton
			-CSS Names with JavaScript Hooks
				--use js- class names
					<div class="site-navigation js-site-navigation"></div> 			CSS
					const nav = document.querySelector('.js-site-navigation') 		JS
			-Write more CSS comments
			https://medium.freecodecamp.org/css-naming-conventions-that-will-save-you-hours-of-debugging-35cea737d849

7p-9p Manila Javascript #28: JavaScript Life at Nokia, Building O, UP Ayala Technohub.
	"State Management with Unstated" by Albert Manuel (JavaScript Developer @ Nokia Technology Center Philippines) 
	"GraphQL with JS" by Joe Gocotano (JavaScript Developer @ Nokia Technology Center Philippines) 
	"Extend Reality with AR" by Archie Herbias (JavaScript Instructor @ Amagi Academy)
	"Tips and Tricks for New Front End Developers" by Thomas Laughlin (CEO @ Amagi Academy)
		Thomas Laughlin

		@ThePracticalDev

		Start from scratch.
		Set goals

		FS dev - I digress. "Full stack is a myth" 
		-specialize

		ES6+ use! 2015

		Yarn> npm

		You don't know everything. And that's okay. 

		"Resume Driven Development" RDD 😂😂😂

		Learn to build the things you want to be paid to build

		[what should I learn first] 
		Don't learn jQuery , learn DOM
		Don"t learn Sass, learn CDS
		Jade < HTML
		Framework < JS
		Handlebars <ES6
		Bootstrap < UI design patterns

		Learn Git
		-Git help everyday

		Start small and grow. Ex: learning english language
		-read, tutorials, small projects, big projects

		[what happens when I visit a site]?? 
		Parsing/tokenization, load scripts, defer/async, etc.

		Learn some style
		Ex: airbnb style guide
		"don't be mean to your teammates" 

		Performance matters, specially in PH
		Performancebudget.io

		Minify or GZip

		REST API design

		Learn JS
		Build stuff (like SPAs) 
		And only then use frameworks

		Follow the masters 
		Read their code
		Learn their lesson 

		Understand FE data flow

		Seriously ES6+

		Use a tool to use modern JS
		Babel + Typescript 

		Learn Node & Yarn 

		Understand async programming 

		Don't stop learning
		Be patient 
		Creativity helps
		EMPATHY

		BrendanEich
		Amasad
		Rmurphey
		KentCDodds

		Fintech PH, MNL analytics, devops PH

   ```

**Thoughts** Feeling worried at the same time excited as I walked past through Nokia's, Bldg. O pantry, at UP Ayala Technohub as my first ever attended meetup.com event: Manila Javascript #28 - The JavaScript Life. I just had a conversation with the meetup organizer, Thomas Laughlin (CEO of Amagi academy), where I asked him something in the sense of "which companies here in the Philippines are like the Google, Facebook, and Airbnb's of Silicon Valley; the landing job success stories in the context of PH". His answer's gist was there was none so far, since the tech scene here in the PH is just building up, almost all the techies here are young ones like me. Nokia and Freelancer.ph are two of three companies he mentioned that I can remember. I have learned from the conversation that there's so much to learn, that perhaps I'll be spending my 20-30s learning to be 'so good they can't ignore you'. One thing I can also remember from him was "avoid tech companies that will make you like a cattle or a carabao". I asked another question, a somehow bad question I guess? "if you will go back to your graduation, will you strive to work for good companies or you'll try to work for known persons who has skills that you like". His answer was it can be both. Thing is, some companies here in PH, like Nokia, even let their European devs to train Filipino devs. One thing I regret was that I wasn't able to say to sir Thomas that "Thank you sir. I can see that you'll have great effect and value in building up the tech scene here in the Philippines, that you'll be remembered for". Hey, after writing this, I guess I also need to write it here that "I'll build the next unicorn tech company here in the PH" (that's my greatest goal as a dev student) #theMagicOfThinkingBig #beSoGoodTheyCantIgnoreYou

**Link(s) to work** Airbnb style guide + same as day 5



### Day 14: July 20, Friday

**Today's Progress**:

```
tweaked specifics to mimic the exact basis to clone
	padding has no effect because max-height was set
		ul li's height to set #topbar height

:hover bottom border color
   ```

**Thoughts** I coded today for just one hour. I'm still grateful with what I've done today since I prioritized to go ask advise my two advisers on my academic journey (undergraduate BS Computer Science). First is my thesis adviser, then my department's (Dept. of Comp Sci) adviser. I got good news on both. For me, what's remarkable today was the proof of getting to act immediately. As Jim Rohn have said, self discipline is 1] the awareness for the constant need for action, 2] and a conscious act to implement that action. If there's considerable time that passes between 1 & 2, then that is called procrastination. Procrastination was my biggest dream killer. After getting good news from my thesis adviser, I took the chance to talk to my dept. adviser this same day. I'm glad I did, I can't tell the details on what happened here. Gist was, I took some time to contemplate what my next step was, and what I'm going to ask for advise, IF I'll still go to my dept. adviser, I took a "forest bath" near our dept. to get some fresh air, (since UP Diliman has many mini forestries) then boom, I guess that helped also. I also had a pick up basketball game tonight, and I also realized that even though I'm training my skills individually everyday, I also need to train my team skills again (need to play 5 vs 5 every week).

![bbc clone topbar progress gif](https://github.com/jbbalderas/100-days-of-code/blob/master/intl/bbc%20clone%20topbar%20progress.gif "Trust the process")

**Link(s) to work** Airbnb style guide + same as day 5


<!--
### Day 15: July 21, Saturday

**Today's Progress**:

```
   ```

**Thoughts**
**Link(s) to work** [link name](url)
   -->
