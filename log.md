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

### Day 2: July 7, Saturday

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
