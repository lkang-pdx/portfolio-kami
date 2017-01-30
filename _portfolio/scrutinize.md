---
layout: post
title: Scrutinize
thumbnail-path: "img/scrutinize.png"
short-description: Built with Rails 5, JavaScript, PostgreSQL

---

{:.center}
![]({{ site.baseurl }}/img/scrutinize.png)

Scrutinize is an analytics service to track events on websites.

### Features:

* Track events on registered websites using a client-side JS snippet
* Capture and save events using a server-side API
* Display the captured event data using [Chartkick](https://github.com/ankane/chartkick)

### Getting Started:

Sign up and register your website on [Scrutinize](https://tranquil-sands-50425.herokuapp.com/).

Add the following JavaScript snippet to the `application.js` file on your website:

```
var scrutinize = {};
  scrutinize.report = function(eventName){
    var event = {event: { name: eventName }};

    var request = new XMLHttpRequest();

    request.open("POST", "https://tranquil-sands-50425.herokuapp.com/api/events", true);

    request.setRequestHeader('Content-Type', 'application/json');

    request.send(JSON.stringify(event));
  };
```
Add the `scrutinize.report` function to the bottom of the desired page. For example, the script below was inserted at the bottom of the About Page.

```
<script type="text/javascript">
    $(document).on("ready page:load", function () {
       scrutinize.report("About Page Visit");
     })
</script>
```
That's it! Scrutinize will then track the events from your registered website.

[Live Demo](https://tranquil-sands-50425.herokuapp.com/)

[GitHub Repo](https://github.com/lkang-pdx/scrutinize)

<!--
## Explanation

Bacon ipsum dolor amet filet mignon meatball spare ribs fatback bacon shankle. Kielbasa andouille fatback salami, boudin bresaola pig alcatra turkey spare ribs jerky. Corned beef bresaola leberkas salami alcatra beef landjaeger venison shank bacon meatloaf beef ribs picanha. Leberkas sausage brisket porchetta shankle prosciutto chicken picanha kielbasa pig kevin t-bone turducken filet mignon jowl.

## Problem

Bacon ipsum dolor amet filet mignon meatball spare ribs fatback bacon shankle. Kielbasa andouille fatback salami, boudin bresaola pig alcatra turkey spare ribs jerky. Corned beef bresaola leberkas salami alcatra beef landjaeger venison shank bacon meatloaf beef ribs picanha. Leberkas sausage brisket porchetta shankle prosciutto chicken picanha kielbasa pig kevin t-bone turducken filet mignon jowl.

## Solution

Bacon ipsum dolor amet filet mignon meatball spare ribs fatback bacon shankle. Kielbasa andouille fatback salami, boudin bresaola pig alcatra turkey spare ribs jerky. Corned beef bresaola leberkas salami alcatra beef landjaeger venison shank bacon meatloaf beef ribs picanha. Leberkas sausage brisket porchetta shankle prosciutto chicken picanha kielbasa pig kevin t-bone turducken filet mignon jowl.

## Results

Bacon ipsum dolor amet filet mignon meatball spare ribs fatback bacon shankle. Kielbasa andouille fatback salami, boudin bresaola pig alcatra turkey spare ribs jerky. Corned beef bresaola leberkas salami alcatra beef landjaeger venison shank bacon meatloaf beef ribs picanha. Leberkas sausage brisket porchetta shankle prosciutto chicken picanha kielbasa pig kevin t-bone turducken filet mignon jowl.

> Bacon ipsum dolor amet filet mignon meatball spare ribs fatback bacon shankle. Kielbasa andouille fatback salami, boudin bresaola pig alcatra turkey spare ribs jerky. Corned beef bresaola leberkas salami alcatra beef landjaeger venison shank bacon meatloaf beef ribs picanha. Leberkas sausage brisket porchetta shankle prosciutto chicken picanha kielbasa pig kevin t-bone turducken filet mignon jowl.

Bacon ipsum dolor amet filet mignon meatball spare ribs fatback bacon shankle. Kielbasa andouille fatback salami, boudin bresaola pig alcatra turkey spare ribs jerky. Corned beef bresaola leberkas salami alcatra beef landjaeger venison shank bacon meatloaf beef ribs picanha. Leberkas sausage brisket porchetta shankle prosciutto chicken picanha kielbasa pig kevin t-bone turducken filet mignon jowl.

## Conclusion

Bacon ipsum dolor amet filet mignon meatball spare ribs fatback bacon shankle. Kielbasa andouille fatback salami, boudin bresaola pig alcatra turkey spare ribs jerky. Corned beef bresaola leberkas salami alcatra beef landjaeger venison shank bacon meatloaf beef ribs picanha. Leberkas sausage brisket porchetta shankle prosciutto chicken picanha kielbasa pig kevin t-bone turducken filet mignon jowl. -->
