# CSS em and rem explained

em is a unit in CSS which we generally use to change font size. "em" refers to the letter "M" as in print terminology -- "em" refers to the width of the letter "M".

em will be relative to its parent's font size. So if a parent container is 16px, then 1em is 16px and 2em is 32px. em's will compound where if a parent container's font size is 2em (32px), then its child's font size of 2em will be 64px.

rem will be relative to the root's font size. This aims as a way to avoid compounding if we don't want that.

## Example using buttons

If we want a button to scale with its font size, we would want to use em. If not, then use rem.

```css
.btn {
    padding: 1em 3em;
}

.btn--small {
    font-size: .5em;
}

.btn--large {
    font-size: 2em;
}
```

The above example will ensure the button's padding scales with the button's font size.

## Why you shouldn't set font-sizes using em

Using ems can cause the compounding effect to destroy your website's layout. It is better to use rem most of the times as it references the root's font size and avoids compounding.