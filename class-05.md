# Class 05 Reading Notes

[Home](https://penjoe.github.io/reading-notes/)

## HTML & CSS Chapter 5: Images

Using images is a great way to give your website more personality. Images can be used simply for decoration or they can be used to relay some sort of information such as a diagram or a chart. Images are inserted into the HTML using the `<img>` tag. You also need to tell the browser where the image is located using the `src` attribute within the `<img>` tag. The location can either be something like an image hosting site or it can just be in an images file as part of the project repository. Aside from the source, you'll also want to add an `alt` attribute and possibly a `title` attribute as well to give more information about the image. Here's what linking an image looks like:
```
<img src="/images/cat.jpeg" alt="picture of a cat" title="Fluffy in all his majestic catliness">
```

While images can be styled right inside the HTML file, more and more often developers are leaving image styling to CSS. This way the HTML file doesn't become overly cluttered. CSS also allows for a deeper level of customization. When using images on a website, it's best to save the image as the proper type. Very colorful photos should always be `.jpeg` whereas photos that are more simple or that have only a few colors are best saved as either `.gif` or `.png` files. Using photoshop or other similar visual editing programs, you can edit the photo as needed and save it as the correct type and also at the correct size you want it for the website to prevent any issues with sizing and image distortion.

## HTML & CSS Chapter 11: Color

Adding color is a very easy way to breathe some life into your web page. With CSS, you can add color to part or all of any element you want. You can specify what color value you want in one of three ways:
* RGB values: This goes off of how much red, blue and green are used using values between 0 and 255. An example would be 50,30,60. 
* Hex codes: These are six-digit codes that represent how much red, blue and green are used, preceded by a `#`. `#ee3e80` is an example of a hex code. 
* Color names: There are 147 predefined color names recognized by browsers, for example 'green' or 'cyan'.
* Click [**HERE**](https://color.adobe.com/create) for a fun tool for picking colors!

Using these three methods, you can change the color value of any element using CSS. There are tons of benefits to changing the color of a document. Contrast can make font easier to read. Certain colors can draw attention to areas you want users to focus on. It also makes it more exciting and user friendly.

With the newest version of CSS, CSS3, you can also adjust color opacity. This is done with the RGBA property whereas the 'A' stands for alpha. Using a number between 0.0 and 1, you can change the opacity of your color to add yet another flavor to your web page. CSS3 has also added a color property called `hsl` and `hsla`. Hsla stands for hue, saturation, lightness and alpha. This just gives a further level of customization for adding color to a web page.

## HTML & CSS Chapter 12: Text