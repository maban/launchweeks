## Adding your launch week

**Not a developer? Open a GitHub issue and we'll do the rest:**

* Company Name
* The name of the launch week
* The launch week's start and end date
* Any links you have about the launch week – landing page, blog posts, tweets, that sort of thing
* A large image we can use on the site to showcase the launch week

**Ok with opening a PR? Here's what to do:**

To add your launch week, you'll need to add 4 files to this repo. Only the first step is essential, the others will make your event look very pretty though.

1. The event metadata in the frontmatter of a markdown file in the `_events` folder
2. The company metadata in the frontmatter of a markdown file in the `_companies` folder
3. A png file that's a banner image for the event, 1500px wide and 400px tall
4. A png file that's an avatar for the company, 400px squared.

### 1: Adding the event

Add a file to the `_events` folder with the filename `companyname-launchnumber.md`` in this format:

```
---
company: Company Name
title: The name of the launch week
launchpage: url to the dedicated page for the launch week (if there is one)
announcement: url to the announcement for the launch week
recap: url to a recap post after the event (if there is one)
image: /media/event-companyname-launchnumber.png
start: Date the event starts in the format YYYY-MM-DD
finish: Date the event finishes in the format YYYY-MM-DD
---
```

Omit any lines you haven't filled out. Here's an example of how that should look:

```
---
company: Hooli
title: Hooli Launch Week 2
launchpage: https://hooli.com/launch-week-2
announcement: https://twitter.com/…
recap: https://hooli.com/blog/launch-week-2-recap
image: /media/event-hooli-2.png
start: 2022-11-23
finish: 2022-12-28
---
```

### 2: Adding the company

If the company is already there, all you need to do is add the event to the event field. If not, add a file to the `_companies_` folder with the filename `companyname.md`` in this format:

```
---
events:
  - The title of the event you've just added
title: Company name
image: /media/avatar-companyname.png
---
```

Omit any lines you haven't filled out. Here's an example of how that should look:

```
---
events:
  - Hooli Launch Week 1
  - Hooli Launch Week 2
title: Hooli
image: /media/avatar-hooli.png
---
```


### 3 and 4: Adding the images

Images are optional but will make the launch event listing look sooooo pretty.

All images go in the `media` folder. For the event, you'll need to add a png file that's 1500px wide and 400px tall. Make sure the file name matches what you put in the event file.

For the company avatar, it's a 400px squared png. You can usually get a good one from LinkedIn.

## Credits

* The site's template is built in [Jekyll](https://jekyllrb.com/).
* Uses components from [Netlify](https://netlify.com/) and [Decap](https://decapcms.org/).
* The reset CSS stylesheet is from [Barebones by Paul Robert Lloyd](https://github.com/paulrobertlloyd/barebones).
* Starry background by from [Transparent Textures](https://www.transparenttextures.com/)