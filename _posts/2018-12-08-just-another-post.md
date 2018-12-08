---
title:  "Just Another Post"
date:   2018-12-08 08:28:16 +0700
---
Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works. This sentence may link to a footnote.[^1]

## GFM Code Blocks

Jekyll also offers powerful support for code snippets in JavaScript. These are
called [fenced code blocks](https://help.github.com/articles/creating-and-highlighting-code-blocks/):

```javascript
export default class OnboardingStartView extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      processing: undefined,
      walkthroughDone: undefined,
    };
  }

```

And Ruby:
```ruby
module Jekyll
  class TagIndex < Page
    def initialize(site, base, dir, tag)
      @site = site
      @base = base
      @dir = dir
      @name = 'index.html'
      self.process(@name)
      self.read_yaml(File.join(base, '_layouts'), 'tag_index.html')
      self.data['tag'] = tag
      tag_title_prefix = site.config['tag_title_prefix'] || 'Tagged: '
      tag_title_suffix = site.config['tag_title_suffix'] || '&#8211;'
      self.data['title'] = "#{tag_title_prefix}#{tag}"
      self.data['description'] = "An archive of posts tagged #{tag}."
    end
  end
end
```

This should show a Gist embed:
<script src="https://gist.github.com/mmistakes/77c68fbb07731a456805a7b473f47841.js"></script>

## Kitchen Sink

This sentence has some _italicized text_. And **this sentence** has some bold
text.

### This is a H3

With some content

#### And this is a H4

Also with some content. How about a numbered list:

1. Some item
2. Another item that goes on for kind of a long time. Another item that goes on for kind of a long time. Another item that goes on for kind of a long time. Another item that goes on for kind of a long time. Another item that goes on for kind of a long time.
3. This one has an unordered sublist:
  * With one item
  * And another
4. And something with a code block:
    ```html
    <script src="https://gist.github.com/mmistakes/77c68fbb07731a456805a7b473f47841.js"></script>
    ```
4. And some final content.

And we can even do unordered lists:

* List item
* Another list item
  * Sublist item
  * Another
* And property indented paragraphs within this list item.
  
  You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

	To have a line break without a paragraph, you will need to use two trailing
  spaces.
  Note that this line is separate, but within the same paragraph.
* A list item with a code block:
    ```html
    <script src="https://gist.github.com/mmistakes/77c68fbb07731a456805a7b473f47841.js"></script>
    ```
* And a final item.

# Header one
## Header two
### Header three
#### Header four
##### Header five

## Blockquotes

Single line blockquote:

> Stay hungry. Stay foolish.

Multi line blockquote with a cite reference:

> People think focus means saying yes to the thing you’ve got to focus on. But that’s not what it means at all. It means saying no to the hundred other good ideas that there are. You have to pick carefully. I’m actually as proud of the things we haven’t done as the things I have done. Innovation is saying no to 1,000 things.
> 
> <q>Steve Jobs — Apple Worldwide Developers' Conference, 1997</q>

Hmmm....Horizontal rule?

---

### Embedded images

And we can have embedded images:

![Screenshot Alt Text](/assets/images/screenshot.png)
![Django Request-Response Cycle](/assets/django_request_response_cycle.png)

## Inline HTML

<dl>
	<dt>Definition list</dt>
	<dd>Is something people use sometimes.</dd>

	<dt>Markdown in HTML</dt>
	<dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>


[^1]: https://example.com
