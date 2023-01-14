# What I learned about SEO and analytics
written by: David Laflamme

Search Engine Optimization (SEO) is used to help websites rank better with search engines. With proper SEOs applied, crawlers identify what to display in search results. They look for content tags such as `<title>, <meta>, <head>, <h1>`, and `<body>`. It's important to properly organize information and not duplicate tags to avoid confusing the crawler. Doing so can result to a lower ranking and cause your site to show up in search results. For example, if a site has more than one `<h1>` tag, the crawler will rank your site lower. 

SEOs can be applied to entire sites or unique pages to prioritize what page shows up first during a search. This helps users find the information more quickly by taking them directly to the intended page rather than a homepage leaving them to search through a site to find what they are initially looking for. With Nuxt, developers can add tags intended for the entire site in the `nuxt.config.js` file and apply the `<head>`,`<meta>`, and other tags to the `<script>` of each subsequent page. There is also the option of making your head tag an object so that you can reuse the information in multiple places and you'll only need to change the object for updates.

Using SEO analytics allows developers to analyze raw data to strategize how to get better results with search engines. This allows marketers to eliminate guessing what customers search so developers can focus on applying what will be most effective. With analytics, it provides user behavior to make more informed decisions on what to prioritize. Developers can leverage several tools such as Google Search Console (GSC), Google Analytics, Ahrefs, Moz Pro, and many other options. Once an account is created, developers and marketers will need to customize their data to make sure to monitor what matters most to strategize on SEOs.

# How I would ideally implement SEO on my site

For my current assignment, I'll implement hypothetical SEO to my site, but to demonstrate how I'd go about it with a real site, I'll use the site I had proposed creating in Assignment 01. My original proposal was to make a brand guideline website for a pretend app called `Workbench` that provides employees with guidance on how to use different brand elements while building marketing content. 

The site would consist of 5 pages:
1. Landing page explaining the brand strategy 
2. How to use the logo
3. Tone of voice
4. Brand colors
5. Media (Illustrations, Photography, and Video) 

Assuming this would be a public site or searchable site within our internal company's websites directory, I'd make the `nuxt.config.js` page contain all elements applicable to the overall brand and additional information such as language and social meta tags specific to each social media platform. I would leave off specific elements such as colors or vocabulary terms used in the tone of voice. In the `<script>` tag of the logo page, I would provide specific terms unique to the logo and purpose. With the colors page I would use unique items such as color names and specifications so that if a user wanted specific data on a color. I would apply the same methodology to the other pages by adding unique SEO specific to those pages' elements. 

Another feature I would use (which I applied to my project), is the `titleTemplate` tag. This allows to specify which page a user is on with a simple sub-title description. Customizing each page would make employees' productivity more efficient as they would spend less time manually searching through the site and get them directly to the information they are looking for.

While this assignment is short and simple, I actually found it impactful. While watching a few youtube videos and reading on pages, I found myself googling more and noticing what these resources were talking about directly in the google search. I hadn't realized until now that search results display what developers intend users to see. This exercise was an eye opening. Thank you, Aaron, for all your help during this entire course. You've truly made a difference to my overall learning experience and you really helped me be successful at actually understanding these concepts. I am forever grateful!