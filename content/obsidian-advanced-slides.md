---
title: Obsidian Advanced Slides
draft: false
tags: 
enableToc: true
---
1. Download Obsidian [here](https://obsidian.md/download) and follow the installation instructions.
2. After installing, open Obsidian.
3. Select 'Create'. Note: A vault in Obsidian is similar to a folder.

	![[Pasted image 20240505164653.png|700]]
4. Name your folder and choose a location for the folder.

	![[Pasted image 20240505164909.png|700]]

# Change Obsidian Theme (Optional)
1. Go to Settings > Appearance > Themes: Manage

	![[Pasted image 20240505170858.png|700]]
1. I prefer the 'Minimal' theme.

	![[Pasted image 20240505170952.png|600]]
1. Select the theme and click 'Install and Use'.

# Set Up Advanced Slides Plugin
1. To create slides in Obsidian, we'll use the Advanced Slides plugin.
2. First, we'll need to turn on Community Plugins from Settings.

	![[Pasted image 20240505165442.png|700]]
1. Next, click 'Browse' and search for 'Advanced Slides'.

	![[Pasted image 20240505165647.png|700]]
1. Click 'Install'. Once it's installed, click 'Enable'.

	![[Pasted image 20240505165920.png|700]]

# Markdown
Obsidian and Advanced Slides is Markdown-based. 

In short, when you put a '#' in front of a line, it is recognized as Heading 1, '##' for Heading 2, and so on.

Basics:
- Heading 1: `#`
- Heading 2: `##`
- Heading 3: `###`
- Bullet points: `-`
- Numbered list: `1.` / `2.` / `3.` etc

Or in Obsidian, you can highlight text, right click and select 'Format' or 'Paragraph' to add formatting to the text.

To insert images:
- Paste an image into the note *OR*
- Drag and drop the image into the note

Recommended settings for images location:
![[Pasted image 20240505182235.png]]


References:
- [Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/)
- [Markdown Basic Guide](https://www.markdownguide.org/basic-syntax/)

# Create Slides
1. Create a note by clicking this icon or using Ctrl+N.

	![[Pasted image 20240505170149.png|700]]
1. Start with the first slide. An example is shown in the image below. 
	- Heading 1 starts with one `#`
	- Heading 2 starts with two `#`
	- Bullet points start with `-`
	- Use `---` to separate the slide from the next one

	![[Pasted image 20240505171646.png|700]]
1. Click this icon to preview the slide.

	![[Pasted image 20240505172052.png|700]]
1. The slide preview will be on the right pane.

	![[Pasted image 20240505172153.png|700]]
1. Here's an example of another slide.

	![[Pasted image 20240505172459.png|700]]

# Change Slide Theme
1. To change the theme your slide, you can specify it at the start of the note, as shown below.

	![[Pasted image 20240505172821.png|700]]
```markdown
---
theme: serif
---
```
2. Built-in themes:
	- black (default)
	- white
	- league
	- beige
	- sky
	- night
	- serif
	- simple
	- solarized
	- blood
	- moon
	- consult
	- css/mattropolis.css

# Other Useful Configuration
- Text align
	- Add this line after the text you want to align: `<!-- element align="left" -->`
- Colours
	- change text highlight colour `<!-- element style="background:red" -->`
	- change font colour `<!-- element style="color:green" -->`
- More than one configuration
	- Separate them by ';' if under same category, e.g., 'style'
	- Separate them by space if different category
	- Example: `<!-- element style="background:grey; color:blue" align="right" -->`
- Example

	![[Pasted image 20240505174140.png|700]]

# Present & Export
1. Click 'Show Grid' to ensure slide content is within the grid.

	![[Pasted image 20240505174646.png|700]]
1. You can directly open the slideshow by clicking 'Open in Browser'

	![[Pasted image 20240505174938.png|700]]
1. Alternatively, you can export it as PDF by selecting 'Print Presentation', then choose 'Save to PDF'.

	![[Pasted image 20240505175337.png|700]]

# Other Plugins
- Menu - A slideout menu plugin for Advanced Slides to quickly jump to any slide by title.
- Overview - Easy navigate to a specific slide
- Chalkboard - Allow writing on slides
- Elapsed Time Bar - Add a progress bar based on the presentation time
- Laser Pointer - A plugin that changes your mouse pointer into a laser pointer. To activate laser pointer press ‘Q’ Button

These plugins can be enabled in Settings > Advanced Slides > Plugins.

![[Pasted image 20240505175854.png|700]]