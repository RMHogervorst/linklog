
using this theme https://cupper-hugo-theme.netlify.app

Goals: 
- it should be supersimple to add a new link
- use the same tags as in kg

aspirations:
    - make the linktype add the correct schema.org type

capture:
    - url / uri / identifyer
    - title
    - what is it about
    - what do i think about it
    - date added

make new posts with `hugo new default.md post/{postname}`

```
difficulties:
  - beginner
  - intermediate
  - advanced
linktypes:
    - paper
    - blogpost
    - bookchapter
    - presentation
    - conference talk
    - book
    - bookseries
    - course
    - course series
tags:
    - inspiration
    - fundamentals
    - mlops
        - ml design
            - ML design patterns
        - versioning
            - data versioning
            - code versioning
            - model versioning
        - coding skills
            - cmdline
            - linux
            - OOP design patterns
            - functional programming
            - python
            - R
            - testing
                - unit testing
                - smoke testing
            - linting
            - CI/CD
        - automation
            - scheduling
            - orchestration
        - monitoring
            - model drift
            - model performance
            - guardrail metrics
        - logging
        - model serving
            - serverless
            - batch
            - continous
        - templating
        - pipelines
            - training pipelines
            - deployment pipelines
            - feature engineering pipelines
    - fairness (ml)
        - justice
        - explainability
    - AI myths
        - robots
    - frameworks
        - torch
        - tensorflow
        - ONNX
```


has shortcodes


{{< note >}}
This is a note! It's something the reader may like to know about but is supplementary to the main content. Use notes when something may be interesting but not critical. You can also *include* **markdown** stuffs like `code`. 
{{< /note >}}

{{< warning >}}
This is a warning! It's about something the reader should be careful to do or to avoid doing. Use warnings when something could go wrong. You can also *include* **markdown** stuffs like `code`.
{{< /warning >}}


{{< blockquote author="Carl Jung" >}}
Even a happy life cannot be without a measure of darkness, and the word happy would lose its meaning if it were not balanced by sadness. It is far better to take things as they come along with patience and equanimity.
{{< /blockquote >}}


{{< expandable label="A section of dummy text" level="2" >}}
Here is some markdown including [a link](https://twitter.com/heydonworks). Donec erat est, feugiat a est sed, aliquet pharetra ipsum. Vivamus in arcu leo. Praesent feugiat, purus a molestie ultrices, libero massa iaculis ante, sit amet accumsan leo eros vel ligula.
{{< /expandable >}}



I don't see the tags, the text is too zoomed in.
There is no overview page on the main page.


can't get this to work

```
 {{ with .Params.difficulties }}
    <div class="level">
      <strong>{{ T "level" }} </strong>
      <ul aria-label="{{ T "aria_label_tags" }}">
        {{ range . }}
          <li>
            {{ $href := print ("difficulties/" | relLangURL) (. | urlize) "/" }}
            <a href="{{ $href }}">{{ . }}</a>
          </li>
    </ul>
  </div>
  {{ end }}
  ```


  ### Notes about podcastfeed
  According to [ausha.co](https://www.ausha.co/blog/creating-an-rss-feed-for-your-podcast/) the feed 
  - needs to be RSS 2.0 RSS
  - feed needs to contain:
    - at least one episode (item)
    - title
    - description
    - link to homepage
  - items need to contain
    - title
    - description
    - pubDate
    - enclosure url with length
    - itunes:duration in minutes:seconds

According to [wiredclip](https://wiredclip.com/podcast-rss-feed/) you need at least
- title
- description
- artwork (3000x3000 px to 1400x1400 px at 72 dpi)
- podcast category
- language
- explicit rating

```XML
<?xml version="1.0" encoding="UTF-8"?>
<rss version="2.0">

<channel>
<title> </title>
<description> </description>
<link> </link>
<item>
    <title> </title>
    <description> </description>
    <pubDate> </pubDate>
    <enclosure url="linktomediafile" type="audio/mpeg" length="234511"/>
    <itunes:duration> </itunes:duration>
</item>
</channel>
</rss>
```

So I guess I should save some of the metadata from the feed
