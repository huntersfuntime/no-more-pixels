# no-more-pixels

### Why should you stop using pixels in CSS? 
- Pixels don't scale
- Font-size does not specifically correlate to pixel size on screen
- One font-family at 16px could have an “A” char 24px high, another font-family at 16px could have an “A” char 26 pixels high.
- Use REM in place of pixels. With REM everything goes off the root font-size of the document.

##### Set your root font-size first 
- By default one REM is 10px;
- So set the root font-size to 10px;
- Change all your other PX to rem.
35px becomes 3.5rem;
125px becomes 12.5rem;

- Now pull up your developer tools and test this out by changing the root font-size and watch it all change.

##### Now change the default root from px to percentage

- By leaving the default root font size as pixels it will remove the custom font in a customers browser.
Some people will increase the font-size in their browser to make it easier to read, by making a default font-size with px it gets rid of that ability.

- The default font-size is 116px. So if we put 100% that would mean the root font-size will be 16px. But we want it to be 10px for the rem. So we take 10/16, which is 62.5%
