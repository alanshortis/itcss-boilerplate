# ITCSS Boilerplate

ITCSS is a way or organising CSS in a logical manner that will reduce issues with specificity, increase maintainability and reduce waste.

It does not require or replace any particular methodology (OOCSS, SMACSS, BEM), syntax, naming conventions or pre-processor.

This boilerplate is just a starting point for any new CSS project. It's extremely light on actual code, and is primarily a template for the file structure.

[This video](https://www.youtube.com/watch?v=1OKZOV-iLj4) from Harry Roberts explains it better than I can.

## Structure

* **Settings**: Global SASS variables, maps, etc.
* **Tools**: SASS functions and mixins. Note: This and the Settings layers can be excluded if you're not using a pre-processor.
* **Generic**: Very far reaching selectors. CSS resets where elements are selected directly and restting non-standard form behaviours.
* **Base**: Default styling on elements without classes, such as typography (`h1`, `h2`, etc) and base elements (`html`, `body`).
* **Components**: Defined parts of the site (navigation, header, footer, carousel) selected with classes, using BEM where appropriate. If it's not obvious what each partial affects, add a comment in your main `.scss` file when it is imported.
* **Trumps**: Overrides, helpers, utilities and shame. The highest specificity and/or classes/properties that must always 'win', using the cascade to beat earlier properties.
