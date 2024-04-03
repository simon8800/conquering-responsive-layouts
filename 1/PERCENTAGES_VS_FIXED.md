# Using percentages and avoiding heights

## Percentages vs fixed widths

When we provide a width to our elements, and the viewport is less wide than the element, we get side-scrolling.

If we don't apply CSS, our HTML is actually responsive already. It's only when we add fixed sizes, that we are dealing with non-responsive elements.

## Percentages on the child

If we apply a fixed width to a child element, it will overflow (spew out of parent element) when the viewport changes past a threshold. In a way, this is a feature that ensures the content can still be accessed and not become blocked by the parent element.

When we apply a percentage, it will be responsive, but still overflow. A lot of the times, setting a width on a child element is not necessary.

## Why it's a good idea to avoid heights

Sometimes we want containers to be a certain height so that it takes up more space for aesthetic reasons. But when we do so, overflow can happen and our page looks broken. Our content adapts to the viewport.

## Challenge

- [] Text should only go up to the midpoint of the container
- [] Text should not overflow when viewport changes