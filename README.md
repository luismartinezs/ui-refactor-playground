# ui-refactor-playground

## What is this?

I created this project to experiment with the concepts in the UX/UI book [ui refactoring](https://refactoringui.com/book/)

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

## Notes of ui refactoring book

REFACTORING UI BOOK

- Start with a feature, not a layout
- Sketch first, detail later
- Design in grayscale, add color later
- Dont design everything upfront, design and code in small cycles
- Designing the smallest useful version you can ship. Coding each extra feature can be very hard.
- Design personality:
	- Font
	- Color
	- Button border radius
	- Language (formal, informal)
- Define a color palette and a set of font sizes beforehand, to limit choice
- Hyerarchy is everything.
- To emphasize something, another option is to depehasaize the other elements
- Use semantic markup (h1...h6), but don't assume you have to use the default brwoser settings. h1 doesnt always need to be large.
- Balance the weight of icons giving them less contrast
- Increase weight to emphasize low contrast elements
- Use a spacing and sizing system for white space, do not use random padding and margin values
	- Use a relative (non linear) scale, eg 16px as base, 4>8>12>16>24>32... when adding space, pick from the spacing system
- Dont make somethin big just to fill the screen
- Design mobile first, the space constraint removes decisions
- Dont take grids (fluid width) as a religion, sometimes it makes sense to make elements a fixed width
	- Elements shouldnt be larger in smaller screens because of the grid. Give elements a max-width and shrink them only when they dont fit the screen
- Large elements shink more than small elements, when going from large screen to small screen
- Always add more space around a group of elemnts than within it
- Make a type size scale (just use the one provided). Stick to px or rem units, not em
- FOnt choice:
	- Basic font choice: -apple-system, Segoe UI, Roboto, Noto Sans, Ubuntu, Cantarell, Helvetica Neue;
	- Google fonts filter for fonts with +10 styles, sort by popularity
	- Steal font choices from good designs
- Make paragraph width around 20-35em (avoi too long lines)
	- Even if content area is wider, still use 20-35em for paragraphs
- Line height depends on font size and paragraph width. Is should be such that finding the next line when reading is easy
- Links: no need to make them all blue, bold them or underline on hover if not part of main user flow
- Center only short texts of 2 or 3 lines
- Right align numbers
- When to tinker with letter-spacing?
	- Narrower headlines
	- Improve all caps legibility
- Color: use HSL
- Increase saturation for lighter and darker colors (mid color 50%, dark and light, 100%)
- When creating a color palette from dark to light, take advantage of perceived brightness (change the hue, not just the brightness and saturation)
- Grey doesnt have to be grey
- Dont rely too much on color, for the color blind. Rely on icons or contrast. USe color to support something design is already saying
- Create 3D illusion:
	- Large shadows for modals
	- Small shadows + highlight for inset / outset shapes
	- Shadow scale defined before hand for differnt elevations
	- Use 2 shadows to represent realistic shadow for elements close to the page
- Overlap elements to create layers
	- When overlapping images, use a border on the top one to avoid clashing
- Crappy photos destroy a design. Use stock photos or hire a photographer
- Avoid image clashing with overlaying text:
	- Add dark overlay
	- Lower image contrast
	- Colorize image
	- Add text shadow and lower a bit image contrast
- Favicons: do not simply scale down the logo. Redraw a simplified verion that looks good at that scale
- Use custom elements: checkboxes, radio butons, links, quotes, icon bullet lists...
- Colorful borders in one side look cool: cards, navigation, alerts, under headlines, top of page...
- Colored backgounds: simply make it more beautiful, distinguish sections, gradients look cool
- https://www.heropatterns.com/
	- Low contrast
- Design emty state for user generate content as a priority. Empty state is user first interacton with site, dont make them boring or after thought
- Fewer borders: separating elemnts is bettwe accomplished with shadows, bg colors and spacing
- Dropdowns, tables, selection by radio buttons... shouldnt look boring. They can be beautiful

How to improve:
- Look at other websites for decisions I wouldnt have made
- Rebuild beautiful interfaces without looking at dev tools

## Exercises

I can just replicate examples in book

- Design and code a feature
- Design something in greyscale
- Design the same thing with 3 styles: corporate feel, playful feel, plain/neutral feel (font, color, border radius, text)
- Make prmary, secondary and tertiary button styles
- Design a card with some content
- Create spacing and sizing system (set of sizes I can use)
- Create a handcrafted type scale
- Find 3 cases of "good fonts" for each: playful sans, neutral sans, serif
- Create a color palette
- Create a menu which has 3D looking buttons and inputs
- Create shadow system
- Make user card (page 196)
- Make card with accented border