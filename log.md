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

**Thoughts** I really though I could finish this project today, I'm now delayed big time, this is just my first ever FCC project. But, I also realized that the next four Responsive Web Design will not really challenge with respect to layout-ing, except the portfolio. What I mean is that, I'm grateful that I'm learning this now, I'm learning alot. I also realized how useful the workflow or shall I say studyflow of "solve problem" -> "can't solve on own" -> "watch tutorials" VS. the typical Watch all tutorials then solve problems/build projects. Wuhooo!
![r1d4 screenshot](https://github.com/jbbalderas/100-days-of-code/blob/master/intl/r1d4%20screenshot.png "Look at 'em CSS. Tried so many things, haha")

**Link(s) to work** [Tribute Page deployed online](https://jim-rohn.netlify.com/)
