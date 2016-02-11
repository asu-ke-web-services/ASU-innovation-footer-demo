# ASU-innovation-footer-demo
This is just a demo of a variation on the innovation footer

You can preview the footer here: https://gios-asu.github.io/ASU-innovation-footer-demo/

## Accepted Variation (Gold)
![Image of variation Desktop](./screenshots/accepted-variation-desktop.png)
![Image of variation Mobile](./screenshots/accepted-variation-mobile.png)

## Original
![Image of original Desktop](./screenshots/original-desktop.png)
![Image of original Desktop](./screenshots/original-mobile.png)

## Proposed Red Variation
![Image of variation Desktop](./screenshots/variation-desktop.png)
![Image of variation Mobile](./screenshots/variation-mobile.png)

*note: In the original only the "Learn to thrive" text is a link, in the variation the image and the white text are both links*


# Implementation
## SASS
```sass
#innovation-bar {
  background-color: #FFC627; /** ASU Gold */
  text-align: right;

  a {
    border-bottom: 0;
    color: black;
    font-size: x-large;
    font-weight: 700;
  }

  a:hover {
    border-bottom: dotted 1px;
    color: #8C1D40; /** ASU Maroon */
  }

  .innovation-footer-image-wrapper {
    height: 0;

    a {
      margin-top: -55px; 
      display: block;
    }

    img { 
      position: relative;
    }
  }
}
## CSS
```css
#innovation-bar {
  background-color: #FFC627; /** ASU Gold */
  text-align: right;
}
#innovation-bar a {
  border-bottom: 0;
  color: black;
  font-size: x-large;
  font-weight: 700;
}
#innovation-bar a:hover {
  border-bottom: dotted 1px;
  color: #8C1D40; /** ASU Maroon */
}
#innovation-bar .innovation-footer-image-wrapper {
  height: 0;
}
#innovation-bar .innovation-footer-image-wrapper a {
  margin-top: -55px; 
  display: block;
}
#innovation-bar .innovation-footer-image-wrapper img { 
  position: relative;
}
```

```
## HTML
```html
<div id="innovation-bar">
  <div class="container">
    <div class="row">
      <div class="col-md-10 space-top-sm space-bot-sm">
        <a href="http://yourfuture.asu.edu/rankings" target="_blank" id="asu-is-number-1-for-innovation">ASU is #1 in the U.S. for Innovation</a>
      </div>
      <div class="hidden-sm hidden-xs col-md-2 innovation-footer-image-wrapper">
         <a href="http://yourfuture.asu.edu/rankings" target="_blank" id="best-colleges-us-news-bage-icon">
          <img src="/path/to/image/best-colleges-us-news-badge.png" alt="Best Colleges U.S. News Most Innovative 2016">
        </a>
      </div>
    </div>
  </div>
</div>
```
