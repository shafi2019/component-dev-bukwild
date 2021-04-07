
Requirements
- This component should have a minimum height of `100vh` but, if the browser is sufficiently short or the content is long, should be able to push past `100vh`.
- Any of the text placements (headline, subhead, etc) should accommodate any length of text without the layout suffering, such as text overlapping other text or being clipped (like by `overflow: hidden`).  In other words, the marquee should just get taller if the text gets long.
- The component should responsively adjust from `320px` up to `1920px` wide.  Everything but the background image should be constrained by a `max-width` of `1440px`.
- The headline and subhead text need to be vertically centered between the menu and the call to action (CTA) box along the bottom.
- The logo, menu, and contact button should all live at the layout level whereas the headline, subhead, CTA box, and background image should all be contained by a marquee component at the page level.  In other words, if one were to navigate to a new page that used this same marquee component, the marquee content would change (new copy, new images, etc) but the layout (logo, menu, etc) would be unaffected.
- The content for the component should be loaded from the provided JSON file and bound to the template via the component’s state/props.  In other words, the content is not hardcoded as template strings.
- Interacting with the upper left menu should change the content in the marquee.
- Don’t use a CSS framework like (Tailwind, Bootstrap, etc).
Judging criteria
- First and foremost, the build should match the design when the browser is the same width as the design.  The design intent should be preserved as elements scale down for narrower browser widths.
- Using of scaling units (vw, %, rem) over fixed units (px) and media queries is preferred.  We would typically use our `fluid()` Stylus function when building with Vue to accomplish this. Ideally, your build uses no media queries except for when changing columns (for instance, moving the subhead under the headline on narrower viewports).
- Elegant handling of the loading of content and image assets will be considered.
- Build-in animation of the component’s elements on the initial render will be considered.
- Easy to understand variable names and comments will be considered.