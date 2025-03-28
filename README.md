# JEDI F.O.R.C.E.

Welcome to the JEDI F.O.R.C.E 

- F – Framework
- O – Optimized
- R – Rendering
- C – Content
- E – Engine

Feel free to reach out to the Agile team for any updates, questions or concerns!

## Installation, Build, Clean and Livereload Server Commands

Please note that depending on your environment you may need ```sudo```

```bundle install```

```bundle exec jekyll clean```

```bundle exec jekyll build --verbose```

```bundle exec jekyll serve --trace --livereload```


# Notes

Please refer to the /test route to see examples of components on one page.

- Internal URIs have been made 'simple', so there is no longer a need to add .html to the end


## Project Folder Structure Notes

### Main build folder

```/docs```

### Table of Contents Data Resource

```docs/_data/resources/table-of-contents.yml``` 

### Main Components

```docs/_includes``` root folder

### Pages Markdown by folder in Main Component root

#### Events

```docs/_includes/events```

#### Mailing List

```docs/_includes/mailing-list```

#### Resources Page

```docs/_includes/resources```

These filesname should match the names used in ```docs/_data/resources/table-of-contents.yml``` 

## New Sidebar top level page

To make a new sidebar page:

1. Duplicate the resources.md page then verbose rename it ( eg. faq.md )
2. Create the same name folder in ```_data```
    - add a table-of-contents.yml (or duplicate from resources)
    - follow the same structure as the resources toc .yml
    - ( eg. _data/faq/table-of-contents.yml)
3. Back in the cloned resources.md page, modify ```{% assign sections = site.data.resources.table-of-contents %}``` to point to the new table of contents page ( eg. ```{% assign sections = site.data.faq.table-of-contents %}```)
4. Create a folder with that newly named page in ```_includes```
    - add .md files matching the table of content yml here
    - eg. ```_includes/faq/intro.md```

## YAML Frontmatter options

```page_title: "Title Here"```
- H1 tag setter

```sidebar: true```
- adds sidebar to page ( currently hardcoded to resources only), we can expand this to pass the _data/[...yml] in the future

```join:true```
- This adds the "Join" button to the top of the page

```post: true```
- This adds the "Post" button to the top of the page
 
## Markdown Rules
- .md files should not have indentation applied when using liquid code, always keep things flush left or the code does not get processed by markdownify

- MD structure can be found in _includes for each section

## Adding a nested MD file

To add a Markdown file on a top level page or in any other markdown file please use this pattern:

- markdown file must be in the root or nested in the _includes folder


```
{% capture replace-this-custom-name %}
{% include /test/test.md%}
{% endcapture %}
{{ replace-this-custom-name | markdownify }}
```

## Table of Contents

- Table of Contents are wired up to the sidebar component

- Table of Contents for each section can be found in /_data as a .yml file, currently we only have /resources/table-of-contents.yml

- Sidebar sections:
    - h1 items are reserved for page titles.
    - add / remove sections from the .yml
    - consider that the root of each is an H2 and the H3s are the sub items
    - make sure to add / remove your main section from the matching /resources.md "assign sections=..." comma separated list (we can automate this during build if you wish)

## Components

The following components are currently available via Liquid code inside Markdown

### List Group

Basic List Group information

Displays basic list item information or other lists in Markdown by capturing the list items using Liquid tags and then rendering them with the custom list group component. Below is an example of how to integrate it:

- separated by line breaks

```
{% capture steering_committee %}
Felix Elwert, Sociological Methods and Research, University of Wisconsin-Madison
Julia Bottesini, JEDI Community Manager (ex officio member)
{% endcapture %}

{% include listgroup.html items=steering_committee %}

```


### List Group Custom (Events)

Displays event information or other specialized lists in Markdown by capturing the list items using Liquid tags and then rendering them with the custom list group component. Below is an example of how to integrate it:

- separated by line breaks

#### Line parsing

- Date and Location: Write it exactly as shown, separated by a comma.
- The | symbol: This divides the two parts, so don’t forget to include it!
- Event Title: After the |, write the full event title.
- Link: Include the link by placing the text in square brackets [ ], followed by the actual link in parentheses ( ).


```
{% capture list_items %}
Friday, September 15, 2023, New York, NY | Exploring Data Transparency in Modern Research [Agenda and slides](https://example.com/link-to-your-event)
{% endcapture %}

{% include listgroup-custom.html items=list_items %}
```

### Image Card

The Image Card component allows you to display an image alongside a description, with support for links embedded in the description. Here’s how you can use the Image Card component in your markdown files:

	1.	Use the | character to separate the image URL, title, description, and an optional link.
	2.	Ensure links are included in markdown or HTML format in the description for proper rendering.

```
{% capture panelists %}
{{ site.baseurl }}/assets/images/event2023/speaker1.png | Speaker Name | This is a description of the speaker. [Learn more](https://example.com)
{{ site.baseurl }}/assets/images/event2023/speaker2.png | Another Speaker | Description about this speaker. [More Info](https://example.com)
{% endcapture %}

{% include card.html items=panelists %}
```

This will render each card with an image, title, and description, allowing for clickable links inside the description.

### Sidebar
- activated in frontmatter

### Table

To use a table you can include this liquid code in you markdown file:

- replace header names (comma separated)
- replace rows, pipe separated "|"

```
{% capture table_headers %}
Column 1, Column 2, Column 3
{% endcapture %}

{% capture table_rows %}
Row 1, Cell 1 | Row 1, Cell 2 | Row 1, Cell 3
Row 2, Cell 1 | Row 2, Cell 2 | Row 2, Cell 3
Row 3, Cell 1 | Row 3, Cell 2 | Row 3, Cell 3
{% endcapture %}

{% include table.html table_headers=table_headers table_rows=table_rows %}
```

### Video

To add a video, include the folloqing liquid code in your markdown file:

- replace the "REPLACE-ME-WITH-EMBED-ID" with the video ID from the YouTube "embed" option found under "Share" in Youtube
- optionally add a custom width and height in pixels if you wish
- optionally add a caption to show below the video

```
{% include video.html video_url="https://www.youtube.com/embed/REPLACE-ME-WITH-EMBED-ID" width="800px" height="450px" caption="Custom size video" %}
```


