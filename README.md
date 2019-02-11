## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/jpthor/test/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Vertical Bar
{% highlight julia %}
using Vega

x = [1, 2, 3, 4, 5]
y = [1, 2, 3, 2, 1]

barplot(x = x, y = y)
{% endhighlight %}

 <div id="vis"></div>

 <script type="text/javascript">
// parse a spec and create a visualization view
function parse(spec) {
  vg.parse.spec(spec, function(chart) { chart({el:"#vis"}).update(); });
}
parse(

{"name":"Vega Visualization","height":450,"padding":"auto","marks":[{"properties":{"enter":{"x":{"field":"x","scale":"x"},"y2":{"field":"y2","scale":"y"},"width":{"offset":-1,"scale":"x","band":true},"fill":{"field":"group","scale":"group"},"y":{"field":"y","scale":"y"}}},"from":{"data":"table"},"type":"rect"}],"axes":[{"properties":{"title":{"fontSize":{"value":14}}},"title":"x","type":"x","scale":"x"},{"titleOffset":40,"properties":{"title":{"fontSize":{"value":14}}},"title":"y","type":"y","scale":"y"}],"data":[{"name":"table","values":[{"x":1,"y2":0,"group":1,"y":1},{"x":2,"y2":0,"group":1,"y":2},{"x":3,"y2":0,"group":1,"y":3},{"x":4,"y2":0,"group":1,"y":2},{"x":5,"y2":0,"group":1,"y":1}]}],"scales":[{"name":"x","range":"width","domain":{"data":"table","field":"x"},"type":"ordinal"},{"name":"y","range":"height","domain":{"data":"table","field":"y"},"type":"linear"},{"name":"group","range":["rgb(166,206,227)","rgb( 31,120,180)","rgb(178,223,138)","rgb( 51,160, 44)","rgb(251,154,153)","rgb(227, 26, 28)","rgb(253,191,111)","rgb(255,127,  0)","rgb(202,178,214)","rgb(106, 61,154)","rgb(255,255,153)","rgb(177, 89, 40)"],"domain":{"data":"table","field":"group"},"type":"ordinal"}],"width":450});
</script>

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/jpthor/test/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.


