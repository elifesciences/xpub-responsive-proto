## Prototypes and guides
- Grids and vertical space: this repo. See it working in a browser at https://elifesciences.github.io/xpub-responsive-proto/web/sample.html
- Design reference https://invis.io/7PMJM3AYUBC#/306987943_wizard-Screen-1

## What this prototype covers
- It demonstrates how components relate to the grid across varying viewport sizes
- It demonstrates how we apply vertical space at eLife (gridUnit). This may need to differ for PubSweet
- It demonstrates components’ behaviour when they are not applied to the grid (app bar)
- It illustrates how we imagine breakpoints will work on the submission wizard so that the same ideas can be applied to other screens

## What this prototype does not cover
- This example is based on the eLife grid, but it doesn’t necessarily propose that as an implementation in this case. A different grid system may behave differently and decisions will need to be made by reviewing the layout of the components on the new system
- PubSweet may have a different approach to the eLife website in regard to a setting vertical space and alignment which will need to be considered

## Guidance
- Our starter point is that our components occupy 12 columns on small devices and then adjust to make use of screen real estate
- Space either side of the grid and gutter is set to 24px
- Component widths are set by specifying numbers of columns rather than fixed values whenever possible
- Components work responsively in a fluid manner with the grid columns and are adjusted to suit the nature of the content, rather than specific device sizes or types (e.g. a text input of 100% browser width is unreasonably wide, so would be set to respond on the grid before reaching this point.). In this way, the UI works on all devices to a certain extent and is as future proof as possible.
- To keep vertical spacing manageable, and to avoid margins collapsing inconveniently, when vertical space is required, it is applied to the bottom of components, never to the top. If an edge case arises where the required vertical space cannot be achieved with this approach, it is acceptable to create a wrapper in order to add more space. This should only be done sparingly. Vertical space may be applied to the top of such a wrapper instead of the bottom if it’s the only way to achieve the desired result. There will almost always be a better way that does not require top spacing.
