# PRE-CSS Day: Bringing Back the Spirit of the Old Web and Keeping CSS Weird

The PRE-CSS Day, introduced by Vasilis in English, was an exciting event held the day before CSS Day.


## Building a website like it's 1999

Sophie Koonin, the Web Engineering Lead at Monzo Bank in London, took the audience on a journey to the past when the web was weirder and had no rules. Sophie's mission is to bring back the spirit of the old web and break free from the uniformity of modern minimalistic design. She reminisced about the days when people built free static sites just for fun, without the influence of social media. 

Sophie encouraged the audience to embrace experimentation and use modern and accessible methods to create weird and unique websites. She showcased examples of animated GIFs, writing HTML in capitals, and demonstrated techniques like getting text via data attributes in CSS. Sophie reminded developers to respect users' preferences by not autoplaying GIFs when specific settings, such as reducing motion, are enabled.

A cool little trick she showed us to get the text via a data attribute in CSS:
```css
content: attr(data-content);
```

## Keep CSS Weird 

Adam Argyle shared insights into color manipulation and the importance of keeping CSS weird. He discussed the differences between HSL (Hue, Saturation, Lightness) and LCH (Lightness, Chroma, Hue) color models. Adam highlighted that the perceptual lightness in LCH is consistent to human eyes, while HSL can be deceiving. He showcased the usage of the "okLCH" function, which allows developers to define colors more accurately using perceptual lightness and other parameters. By embracing the weirdness of CSS and exploring alternative color models, developers can create visually interesting and unique designs.

```css
background-color: oklch(99%, .05, 320);
// lightness, chroma, hue
```
