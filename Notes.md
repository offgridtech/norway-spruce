# Important Notes

We are going to keep only one page of notes here, so we don't waste time taking notes in all of the code as we go.

## Component Based CSS

You want to build all of your components like the nav bar, banner/hero section, buttons, input fields + buttons, badges, cards, links, grids, media objects, testimonials, callout components (take action). You build these in isolation as if nothing else exists, and then you put them together in the end.

## Color Palette

Primary, secondary, and accent colors.

For the Norway Spruce page, let's make green the primary color with different shades of green as secondary colors. An accent color sticks out, like red, orange or yellow. Play around with the accent colors to see what would look best with the different shades of green.

## Minimize the Number of Fonts

Page load times decreases when you have less stuff loading, so stick with the least amount of font styles possible. Every variation of a font becomes a separate font file, so keep everything simple and minimal.

One thing to note is that variable font files have multiple types of a font included in only one file. Something to look for so you make less HTTP requests, and also you can link multiple font types without increasing size.

## Minimize the Number of <links> in the HTML

Import normalize.css into your main CSS file at the top using @import "./normalize.css". The less links you have in the markup, the faster it will be. During the build process with Parcel, it will combine the CSS file and normalize.

## Use the W3 Validation Tool

You copy and paste or attach your HTML and CSS, and it will tell you what you need to know to fix it. Do this before performing a build and deploying to production. The better your code is as per the validator, the higher ranking you will get in search engines.

## Use a Build Tool (Parcel)

Build a Parcel local development server to test using the CLI with `node_modules/.bin/parcel index.html`, and see how it looks on your local machine. Then, do a production build with `node_modules/.bin/parcel build index.html` to remove all the comments, spacing, etc, from all of your files, and then it will dump new optimized files into .dist.

## Use a PaaS to Bypass Infrastructure & Security

Netlify and Firebase are the hot ones right now. Compare them. You connect your Github with these services so that when you push your code to your remote repo in Github, these PaaS services are listening, and will automatically build with the new changes. All you have to do is code, and you don't have to worry about any backend stuff. Make the customer pay for it or get some sort of professional account to store them all in your own.

## Use Performance Measurement Tools

web.dev (PageSpeed Insights) or Lighthouse will scan your website that has been deployed, and give you feedback about what you can do to optimize it better.
