# flex-grid

A simple grid built using LESS and flexbox. Using CSS Grid is a much better approach, but this was created before I learned Grid.

## Major Breakpoints

- `@bp-min: 320px;`
- `@bp-xs: 480px;`
- `@bp-sm: 540px;`
- `@bp-med: 768px;`
- `@bp-lg: 990px;`
- `@bp-xl: 1240px;`
- `@bp-xxl: 1440px;`
- `@bp-max: 1920px;`

## Row Selectors

<dl>
  <dt>`.l-flex`</dt>
  <dd>Block: Unstack around the grid row</dd>

  <dt>`.l-flex--row-min`</dt>
  <dd>Modifier: Unstack at smallest major breakpoint</dd>

  <dt>`.l-flex--row-xs`</dt>
  <dd>Modifier: Unstack at the extra small breakpoint major breakpoint</dd>

  <dt>`.l-flex--row-sm`</dt>
  <dd>Modifier: Unstack at the small breakpoint major breakpoint</dd>

  <dt>`.l-flex--row-med`</dt>
  <dd>Modifier: Unstack at the medium breakpoint major breakpoint</dd>

  <dt>`.l-flex--row-lg`</dt>
  <dd>Modifier: Unstack at the large breakpoint major breakpoint</dd>

  <dt>`.l-flex--row-xl`</dt>
  <dd>Modifier: Unstack at the extra large breakpoint major breakpoint</dd>

  <dt>`.l-flex--row-xxl`</dt>
  <dd>Modifier: Unstack at the extra extra large breakpoint major breakpoint</dd>

  <dt>`.flex--row-max`</dt>
  <dd>Modifier: Unstack at the maximum major breakpoint</dd>

  <dt>`.l-flex--no-row-gap`</dt>
  <dd>Remove the top and bottom margin from rows</dd>

  <dt>`.l-flex--no-col-gap`</dt>
  <dd>Remove the left and right margin from columns</dd>

  <dt>`.l-flex--no-gap`</dt>
  <dd>Remove the top and bottom margin from rows and the left and right margin from columns</dd>
</dl>

## Column Selectors

<dl>
  <dt>`.l-flex__none`</dt>
  <dd>Column will be width of content</dd>

  <dt>`.l-flex__eighth`</dt>
  <dd>Column width is 1/8th of the screen</dd>

  <dt>`.l-flex__quarter`</dt>
  <dd>Column width is 1/4 of the screen</dd>

  <dt>`.l-flex__third`</dt>
  <dd>Column width is 1/3 of the screen</dd>

  <dt>`.l-flex__half`</dt>
  <dd>Column width is 1/2 of the screen</dd>

  <dt>`.l-flex__two-third`</dt>
  <dd>Column width is 2/3 of the screen</dd>

  <dt>`.l-flex__three-quarter`</dt>
  <dd>Column width is 3/4 of the screen</dd>

  <dt>`.l-flex__full`</dt>
  <dd>Column width is 100% of the screen</dd>
</dl>

## Description

Since this grid is based on flexbox there are many ways it can be implemented. The example can be found on CodePen. It is not a 12 or 16 column grid. Due to it's simplicity, the code required to create the layout has a small footprint compared to many other grids.

This was created before CSS Grid was fully released to meet my own project needs and personal interest in writing a grid. Most of my projects didn't have a need to change the layout at different breakpoints, e.g. 6 column at a medium breakpoint and 4 column at a small breakpoint. These are great options provided by other grid systems, but I rarely found the need on my projects.

Also, most the projects I had been working on were developed using LESS and most of the Grid implementations from popular style guides/design systems are writting in SCSS.
