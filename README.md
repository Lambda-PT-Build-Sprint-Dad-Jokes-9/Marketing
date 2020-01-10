To contribute to this project, please follow the guidelines in this readme.
DadJokes Marketing Page is a static html website with some minimal javascript functionality. 
The html and css is largely shared across the marketing pages, inheriting the same navbar, jumbotron, 
and footer. Each page has a section that varies from the others, and if you want to add more 
information to the marketing pages, make a new html file, copy the common layout html sections, and 
build from there.


The styling is compiled using less, so in your terminal, input  ``less-watch-compiler less css index.less`` to 
get the compiler up and running.


From there, the main file hosting the styling is the ``homepage.less`` file. 


In the variables.less file, you can see the different media settings for responsive design.


If you do add pages to the website, you will have to manually changes the settings in the burger.less file, 
which contains the styling for the hamburger menu. The most pertinent setting to change is the 
``.wrapper { height: 50px}`` section. For each new site you add to the burger menu, increase its height by 
25px. To add the items in the hamburger menu, navigate to the <header> section, and locate the section 
with the class “menu menu-off”, and add a div with the following format ``<div><a 
href=”urlhere”>text</a></div>`` for each new link you wish to put there.


The jumbotron and navbar uses a slightly customized version of material design. The div hosting the text 
and app button are custom, and the styling can be found in the homepage.less file. Also, the hamburger 
menu is customized as well, with the relevant files being burger.less and a small snippet of javascript in 
the main.js file. See https://material.io/develop/web/components/cards/ for documentation on these 
components.


For the information cards used in the index and about-us pages, they use flexbox. It works well for 
responsive text and will have no issue handling extra cards if you wish to add them. Use/change the 
`features-info` and `info-container` classes to add/change feature cards in the main page,  and the 
`features-container` and `about-container` classes  to add/change person cards in the about-us page.









Product Vision Document

- What problem does your app solve?
It solves the problem of not having enough dad jokes to annoy your family with.

- Be as specific as possible; how does your app solve the problem? 

Connects users so that they can share their jokes with one another. Offers the ability to create personal accounts to create jokes and offer attribution for their creation. A platform to share all the “Dad Jokes” with the world! Enables users to be able to also edit/delete their jokes if necessary.

- What is the mission statement?
Dads Jokes has got you covered with a real zinger for every situation! 
Features

- What features are required for your minimum viable product?

[ ] - User can view dad jokes listed as 'public' without having an account (being authenticated)

[ ] - User can sign up as by providing a unique username and a password that will serve as their login/authentication credentials. 

[ ] - An authenticated user has the ability to view, create, edit and delete jokes. 

(mobile, web): A "jokes" page/view where they can:

---View all public (private as well if the user is logged) jokes

---If logged in, select a joke from the list and present a detail view where they could edit the joke

[ ] - Create a joke. A joke must have at minimum the following properties:
  	* `question` - String
	* `joke/answer` - String

[ ] - Edit a joke.

[ ] - Delete a joke.

- What features may you wish to put in a future release?

On load it would return a random roll of 10 jokes
Random dad joke of the day
Categorize dad jokes
Social sharing (deep linking)
Upvoting (community responses)
Content filtering 


- What do the top 3 similar apps do for their users? 
Frameworks - Libraries

- What 3rd party frameworks/libraries are you considering using?

		-for BE: Node JS/Express/Knex, morgan, helmet
		-for FE React JS, Redux/Context, ReactStrap, Styled Components, Axios, React-Router, Google Fonts, Font Awesome
		-for Marketing, LESS, Html, GoogleFonts, Font Awesome 
	
 
- Do APIs require you to contact its maintainer to gain access? No. 
- Are you required to pay to use the API?
	
--- Not right off the bat, but if we can get to stretch will work in stripe

- Have you considered using Apple Frameworks? (MapKit, Healthkit, ARKit?) No.

Target Audience

- Who is your target audience? Be specific. 
People who want to say dad jokes. Everyone! 


Research

- Research thoroughly before writing a single line of code. Solidify the features of your app conceptually before implementation. Spend the weekend researching so you can hit the ground running on Monday.

Fmylife.com - Social stories about how hard things about their lives have been
Niceonedad.com - Pulls up one joke at a time, and then you can hit next and it pulls up another random joke
Fatherly.com - Had jokes separated by events or topics (categorized) 
Prototype Key Feature(s)

- This is the “bread and butter” of the app, this is what makes your app yours. Calculate how long it takes to implement these features and triple the time estimated. That way you’ll have plenty of time to finish. It is preferred to drop features and spend more time working on your MVP features if needed.


