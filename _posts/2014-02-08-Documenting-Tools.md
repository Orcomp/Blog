---
layout : post
title : Documentating Tools
category : Manual
tags :
  - Documentation
  - Requirement Writing
  - Tools
---

Here are some tools I find extremely helpful when writing requirements and documentation.

I have tried a lot of different apps over the years and have found these to be the best for my needs.

My main criteria for selecting these tools are:
- Easy to use (after a short learning period).
- Productive (the tool must not get in the way of what I am writing).
- Can be **version controlled**. (i.e. saves files to text format. This is **really** important for me.)

### MardownPad (Markdown editor and viewer)

Website: [http://markdownpad.com/](http://markdownpad.com/)

I try and write all my docs and requirements in [markdown](http://daringfireball.net/projects/markdown/syntax) format. ([CheatSheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)).

MarkdownPad works well for me. I use the GitHub flavored Markdown (Offline) setting.

![Settings]({{site.url}}/img/DocumentingTools/markdownPadSettings.png)

### TpX (Illustration tool)

Webiste: [http://tpx.sourceforge.net/](http://tpx.sourceforge.net/)

For drawing illustrations quickly and efficiently. (Make sure you learn the [shortcut keys](http://tpx.sourceforge.net/tpx_using_mouse_for_editing.htm)).

I can draw illustrations really fast with this tool. It is not the most polished illustration tool out there and it does not have thousands of options, but it is hands down the most productive for me.

(It has not be updated in a long time but it does not need to...)

### PlantUML (UML diagrams)

Website: [http://plantuml.sourceforge.net/](http://plantuml.sourceforge.net/)

(Yea.. the website looks terrible, but the tool is great :)

- Excellent flowcharting capabilities.

You may want to use [plantumlqeditor](http://sourceforge.net/projects/plantumlqeditor/) as an editor and viewer.

UML cheatsheets: [cheatsheet1](http://loufranco.com/wp-content/uploads/2012/11/cheatsheet.pdf), [cheatsheet2](http://www.digilife.be/quickreferences/QRC/UML%20Reference%20Card.pdf).

### GreenShot (Screen capture)

Website: [http://getgreenshot.org/](http://getgreenshot.org/)

Best free screen capture out there. Simple and does what it is supposed to really well.

It has basic (but more than adequate) picture annotating tools. 
Again it is fast and stays out the way.Perfect!

For me Greenshot is hands down the best free screen capture application available on Windows.

## Summary

That is it! you only need 4 tools to be really productive at writing documentation and requirements.

All of these tools (except Greeshot) will produce text documents that can easily be version controlled and saved to a git repository.

> A picture is worth a thousand words.
> 
> A good annotated picture (or illustration) is worth even more :)

# Requirement Writing Tips

The key to requirement writing is realizing that describing the problem **accurately** (yet succinctly) will get you more than half way closer to the **right** solution.

That is why good requirements are so important and valuable. The wrong requirement can cost thousands if not hundreds of thousands of dollars. 

## Process

1. Deconstruct the problem first, starting from a very high level.
2. Determine the major building blocks or decision points.
3. Determine the inputs and outputs for each building block.
4. Try and abstract the problem and decouple the building blocks as much as possible.
5. Then drill down into each major building block repeating steps 1, 2, 3 and 4.

6. Once you have reached the lowest level building blocks. Then you can start writing the requirements for each lowest level building block.

## Execution

- Keep it short (less than a page).
	- keep sentences short. (Use as few words as possible.)
- Keep it simple.
	- Use bullet points.
- Always include at least one illustration or diagram. (but not too many.)

**Notes**:

- If you can not keep a requirement short or simple it is generally a good indication you need to split your requirement into smaller requirements. (Go back to step 5. in the Process section.)

- Do not try and make pictures and illustrations beautiful. They only need to convey key pieces of information. Keep them simple.

**Fact**: Writing good requirements is hard work and usually take time and a few iterations.

> Thats been one of my mantras - focus and simplicity. Simple can be harder than complex: You have to work hard to get your thinking clean to make it simple. But its worth it in the end because once you get there, you can move mountains.
>
> **Steve Jobs**


**Hint**: Once requirements are written and implemented, they can be turned into documentation.

# Documentation Writing tips

- Consolidate all requirements.
- Use flowcharts to illustrate the main logic, building blocks and decision points.