# Imdex CSS/SASS style guide
> A list of recommended CSS/SASS format rules

## Class names
- Avoid excessive and arbitrary shorthand notation, use meaningful names.
- Keep classes lowercase and use dashes (not underscores or camelCase). Dashes serve as natural breaks in related class.
```
.reflex-logo-text {
    font: oblique bold 4em 'Reflex-Font';
    color: $reflex-blue !important;
    text-shadow: 2px 2px 2px #DDDDDD;
    letter-spacing: -2px;
}
```
## Syntax
- Include one space after **:** for each declaration.
- Include one space before the opening brace of declaration blocks for legibility.
- When grouping selectors, keep individual selectors to a single line.
```
input.ng-invalid,
input.input-validation-error {
  border: 1px solid #FF9595;
}
```
- End all declarations with a semi-colon.
- Place closing braces of declaration blocks on a new line.
- Each declaration should appear on its own line for more accurate error reporting.
```
.logo-icon-group {
    padding-left: 75px;
    margin-bottom: -20px;

    > img {
        max-width: 45px;
        margin-right: 10px;
    }
}
```
- Avoid specifying units for zero values.
- Don't prefix property values or color parameters with a leading zero.
```
#sidebar-menu {
    padding: 0;

    li {
        border-bottom: 1px solid rgba(255, 255, 255, .2);
    }
}
```
- Use shorthand hex values where available.
## Selectors
- Use classes over generic element tag for optimum rendering performance.
- Keep selectors short and strive to limit the number of elements in each selector to three.
- Scope classes to the closest parent only when necessary (e.g., when not using prefixed classes).
## Media query
- Place media queries as close to their relevant rule sets whenever possible. Don't bundle them all in a separate stylesheet or at the end of the document.
## Shorthand notation
- Strive to limit use of shorthand declarations to instances where you must explicitly set all the available values.
```
.wrapper {
    margin-top: 90px;
    display: inline-block;
    padding-left: 15px;
    width: 100%;
}
```
