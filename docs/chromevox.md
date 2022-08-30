# Using ChromeVox for basic tests

Learning to use a screenreader properly is well outside the scope of this project but having a basic understanding of how a screenreader can interact with a webpage is helpful.  

ChromeVox is a screenreader which integrates into the Chrome browser. It is free to use and works with mathematical text encoded in webpages using MathJax. We will use a restricted mode of the ChromeVox screenreader which is easier for a complete beginner.

### Example of ChromeVox reading maths

<iframe width="560" height="315" src="https://www.youtube.com/embed/o059smdYHMo?rel=0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Install ChromeVox

To install ChromeVox:

* Start Chrome
* Go to [the ChromeVox extension](https://chrome.google.com/webstore/detail/screen-reader/kgejglhpjiefppelpmljglcjbhoiplfn?hl=en)
* Click on the Add to Chrome button
* Go to [Chrome extension list](chrome://extensions/), you should be able to see ChromeVox. Here you will find a slider to switch the extension on and off. You will want to switch it off whenever you are not intending to use it!

When ChromeVox is running you can change or manage [ChromeVox options](chrome-extension://kgejglhpjiefppelpmljglcjbhoiplfn/chromevox/background/options.html) but this tutorial does not depend on any changes. If you have previously installed ChromeVox and the below does not work then you may wish to check that you are using the Classic keymap and Reset current keymap.  

### Using ChromeVox

Please note that students will **certainly** have a screenreader more suited to education and employment than ChromeVox and that no student should be asked to change or acquire a skillset in a new screenreader without very good reason and plenty of advance notice. 

These are instructions are not intended to teach you how to use a screenreader and they are not suitable for someone who usually uses a screenreader. These instructions exist solely to help you to understand how a structured webpage, equation or interactive diagram might sound to a screenreader user.

To use ChromeVox to read mathematical text correctly you **must** use the keyboard, not the mouse. Mathematics will be read incorrectly if the mouse is used.

1. Enable the ChromeVox addon with the example page, or your own page, open.
2. ChromeVox will start if it is enabled. 
   * To stop ChromeVox from finishing the current output press **Ctrl**
   * When you have finished using ChromeVox you will want to disable it using the slider on the [Chrome extension list](chrome://extensions/). It is possible to switch it off but to leave it enabled but this is beyond the scope of this introduction. 
3. ChromeVox has a mode called sticky mode. We are only going to use this mode as it is easy for an untrained user. You cannot fill in forms or edit when in this mode. 
   * To get in or out of scan mode press **Insert** TWICE on Windows or Linux or **left Command key** TWICE on Mac OS
   * Please remember that there are lots of things a screenreader can do, ChromeVox included, that we are **not** teaching you how to do!
4. Try not to use the mouse! Once in sticky mode use the below commands to explore the page. Try to move through the document in different ways to 'scan' it. 
5. Try to read a mathematical expression. Can you "enter" the mathematical expression and explore it?   
6. Try to interact with any interactive diagrams. Listen carefully for the instructions on how to do this.  

#### General keyboard commands

| Key press   	  | What will happen?	       	       	     	      	|
| --------------- |-----------------------------------------------------|
| Enter		  | Activate current item				|
| Tab		  | Jump to next focusable item				|
| Shift + Tab	  | Jump to previous focusable item			|
| Down/Up	  | Navigate forwards/backwards		   		|
| Right/Left	  | Navigate forwards/backwards at a more detailed level|
| Backslash	  | Enter table or equation exploration			|
| Backspace		  | Exit table or equation exploration			|
| N		  | Next (follow by any of the below type commands)	|    				     		|
| P		  | Previous (follow by any of the below type commands)	|
| H		  | Heading  	     	       	   	      		|
| n in {1,..,9}	  | Heading at level n					|
| L		  | Link						|
| T		  | Table						|
| O		  | List						|
| I		  | List item						|

#### Exploring tables

In sticky mode, 

* use backslash to enter a table;
* use backspace to exit a table;
* use navigation left/right/up/down to move between cells and
* inside the table use the below keypresses to explore.

| Key press   	  | What will happen?	       	       	|
| --------------- |-----------------------------------------------------|
| T H		  | Announce the headers of the current cell		|
| T L     | Announce the current cell coordinates       |
| T [     | Go to the beginning of the table            |
| T ]     | Go to the end of the table                  |
| T ;     | Go to the beginning of the current row      |
| T #     | Go to the end of the current row            |
| T ,     | Go to the beginning of the current column   |
| T .     | Go to the end of the current column         


#### Exploring mathematical expressions

In sticky mode, 

* use backslash to enter an expression;
* use backspace to exit an expression;
* inside the expression use the below keypresses to explore.

| Key press   	  | What will happen?	       	       	|
| --------------- |-----------------------------------------------------|
| Down/Up		  | Navigate forwards/backwards		|
| =           | Increase granularity |
| -           | Decrease granularity |
| M S         | Toggle semantic mode |

In semantic mode, in multi-line displayed equations, the reading will not announce the cell location of the current element but will instead read the maths as expressions. 


## Arc length 
We often need to know the length of a curve between two points,
e.g. what is the length of the ropes holding Clifton suspension bridge (see Exercise Sheet 3).

### Visualisation 

Given a curve $y=y(x)$

<iframe src="https://www.desmos.com/calculator/fd09vdozmt?embed" width="100%" height="400px" data-external="1"></iframe>

Let $S$ be the arc length and  $\Delta S$ a short section of it.

<iframe src="https://www.desmos.com/calculator/qvrxafeubg?embed" width="100%" height="400px" data-external="1"></iframe>

### Derivation of Arc Length

By Pythagoras' Theorem,
$$
\Delta S^2 \approx \Delta x^2+\Delta y^2
\qquad \Rightarrow\qquad
\left(\dfrac{\Delta S}{\Delta x}\right)^2 \approx 1+\left(\dfrac{\Delta y}{\Delta x}\right)^2
$$
As $\Delta x\to0$ this becomes an identity
$$
\left(\dfrac{dS}{dx}\right)^2 = 1+\left(\dfrac{dy}{dx}\right)^2
\qquad\Rightarrow\qquad
\dfrac{dS}{dx} = \sqrt{1+\left(\dfrac{dy}{dx}\right)^2}
$$
The arclength between $x=a$ and $x=b$ is then
$$
\begin{aligned}
  S(a,b) &= \int_a^b\dfrac{dS}{dx}dx\\
  &= \int_a^b\sqrt{1+\left(\dfrac{dy}{dx}\right)^2}dx.
\end{aligned}
$$




<!--## Read&Write addon to Chrome

It is also possible to use the [TextHelp Read&Write](https://chrome.google.com/webstore/detail/readwrite-for-google-chro/inoeonmfapjbbkmdafoankkfajkcphgd) addon to Chrome to read mathematical content. It is easier to use to test content as it is used with a mouse and you simply hover over text. The speech functionality remains free after the end of the trial period. However, this addon will only work on **live** webpages and so we are not able to use it to test output without uploading it somewhere. If one is intending to distribute pages to students via a virtual learning environment then upload to this environment for testing may be preferable.  

### Installation

<iframe width="560" height="315" src="https://www.youtube.com/embed/i8fM8Z23h00" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Example of Read&Write reading maths

<iframe width="560" height="315" src="https://www.youtube.com/embed/GTnyNJ4hKp0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>-->

[Return to plan](index.html)