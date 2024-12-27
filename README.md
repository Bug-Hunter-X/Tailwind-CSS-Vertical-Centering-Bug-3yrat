# Tailwind CSS Vertical Centering Bug
This repository demonstrates a subtle bug in Tailwind CSS's vertical centering capabilities when the parent element's height is not explicitly set.

## Bug Description
The `flex items-center justify-center` combination usually centers elements effectively. However, under certain conditions, particularly when the parent element's height is dynamic or not explicitly defined using `h-screen` or a similar height-setting class, the vertical centering might fail.  The issue often manifests in responsive layouts or when the parent container's height depends on its content.

## Reproduction
1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe that the blue box isn't perfectly vertically centered in some viewport sizes.

## Solution
The solution involves explicitly setting the height of the parent container to ensure the `items-center` property can function correctly. You can achieve this using various techniques including fixed height, `min-h-screen`, `vh` units, or other methods suitable for your layout's context.
