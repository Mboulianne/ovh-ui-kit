# oui-table

<component-status cx-design="partial" ux="prototype"></component-status>

oui-table is a package which provides styles for the table component.

## Installation

```less
  @import 'oui-table/table';
```

## Usage

```html:preview
<table class="oui-table">
  <thead class="oui-table__headers">
    <tr>
      <th class="oui-table__header oui-table__cell_sortable" tabindex="0">Filename</th>
      <th class="oui-table__header oui-table__cell_sortable-asc oui-table__cell_sorted" tabindex="0">Id</th>
      <th class="oui-table__header oui-table__cell_sortable-asc" tabindex="0">Size</th>
      <th class="oui-table__header oui-table__cell_sortable-desc" tabindex="0">Creation</th>
    </tr>
  </thead>
  <tbody class="oui-table__body">
    <tr class="oui-table__row" tabindex="0">
      <td data-title="Filename" class="oui-table__cell">abc</td>
      <td data-title="Id" class="oui-table__cell">1</td>
      <td data-title="Size" class="oui-table__cell">123 KB</td>
      <td data-title="Creation" class="oui-table__cell">Sun Mar 19 19:53:24 2017</td>
    </tr>
    <tr class="oui-table__row" tabindex="0">
      <td data-title="Filename" class="oui-table__cell">abc</td>
      <td data-title="Id" class="oui-table__cell">2</td>
      <td data-title="Size" class="oui-table__cell">123 KB</td>
      <td data-title="Creation" class="oui-table__cell">Sun Mar 19 19:53:24 2017</td>
    </tr>
    <tr class="oui-table__row" tabindex="0">
      <td data-title="Filename" class="oui-table__cell">abc</td>
      <td data-title="Id" class="oui-table__cell">3</td>
      <td data-title="Size" class="oui-table__cell">123 KB</td>
      <td data-title="Creation" class="oui-table__cell">Sun Mar 19 19:53:24 2017</td>
    </tr>
  </tbody>
</table>
```

### Responsive

```html:preview
<table class="oui-table oui-table_responsive">
  <thead class="oui-table__headers">
    <tr>
      <th class="oui-table__header oui-table__cell_sortable" tabindex="0">Filename</th>
      <th class="oui-table__header oui-table__cell_sortable-asc oui-table__cell_sorted" tabindex="0">Id</th>
      <th class="oui-table__header oui-table__cell_sortable-asc" tabindex="0">Size</th>
      <th class="oui-table__header oui-table__cell_sortable-desc" tabindex="0">Creation</th>
    </tr>
  </thead>
  <tbody class="oui-table__body">
    <tr class="oui-table__row" tabindex="0">
      <td data-title="Filename" class="oui-table__cell">abc
        <i role="button" class="oui-icon oui-icon-chevron-right oui-table__expand-button"></i>
      </td>
      <td data-title="Id" class="oui-table__cell">1</td>
      <td data-title="Size" class="oui-table__cell">123 KB</td>
      <td data-title="Creation" class="oui-table__cell">Sun Mar 19 19:53:24 2017</td>
    </tr>
    <tr class="oui-table__row oui-table__row_closed" tabindex="0">
      <td data-title="Filename" class="oui-table__cell">abc
        <i role="button" class="oui-icon oui-icon-chevron-right oui-table__expand-button"></i>
      </td>
      <td data-title="Id" class="oui-table__cell">2</td>
      <td data-title="Size" class="oui-table__cell">123 KB</td>
      <td data-title="Creation" class="oui-table__cell">Sun Mar 19 19:53:24 2017</td>
    </tr>
    <tr class="oui-table__row oui-table__row_closed" tabindex="0">
      <td data-title="Filename" class="oui-table__cell">abc
        <i role="button" class="oui-icon oui-icon-chevron-right oui-table__expand-button"></i>
      </td>
      <td data-title="Id" class="oui-table__cell">3</td>
      <td data-title="Size" class="oui-table__cell">123 KB</td>
      <td data-title="Creation" class="oui-table__cell">Sun Mar 19 19:53:24 2017</td>
    </tr>
    <tr class="oui-table__row oui-table__row_closed" tabindex="0">
      <td data-title="Filename" class="oui-table__cell">abc
        <i role="button" class="oui-icon oui-icon-chevron-right oui-table__expand-button"></i>
      </td>
      <td data-title="Id" class="oui-table__cell">4</td>
      <td data-title="Size" class="oui-table__cell">123 KB</td>
      <td data-title="Creation" class="oui-table__cell">Sun Mar 19 19:53:24 2017</td>
    </tr>
    <tr class="oui-table__row oui-table__row_closed" tabindex="0">
      <td data-title="Filename" class="oui-table__cell">abc
        <i role="button" class="oui-icon oui-icon-chevron-right oui-table__expand-button"></i>
      </td>
      <td data-title="Id" class="oui-table__cell">5</td>
      <td data-title="Size" class="oui-table__cell">123 KB</td>
      <td data-title="Creation" class="oui-table__cell">Sun Mar 19 19:53:24 2017</td>
    </tr>
    <tr class="oui-table__row oui-table__row_closed" tabindex="0">
      <td data-title="Filename" class="oui-table__cell">abc</td>
      <td data-title="Id" class="oui-table__cell">6</td>
      <td data-title="Size" class="oui-table__cell">123 KB</td>
      <td data-title="Creation" class="oui-table__cell">Sun Mar 19 19:53:24 2017</td>
    </tr>
  </tbody>
</table>
```

### Basic HTML table

```
┌ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ┐
│ oui-table [table]             │───────────────────────────────────────────────────────────────┐
├ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ┘                                                               │
│┌oui-table__headers [thead]───────────────────────────────────────────────────────────────────┐│
││┌oui-table__row [tr]────────────────────────────────────────────────────────────────────────┐││
│││┌oui-table__header [th]──────┐┌oui-table__header [th]───────┐┌oui-table__header [th]──────┐│││
││││                            ││                             ││                            ││││
││││                            ││                             ││                            ││││
││││                            ││                             ││                            ││││
│││└────────────────────────────┘└─────────────────────────────┘└────────────────────────────┘│││
││└───────────────────────────────────────────────────────────────────────────────────────────┘││
│└─────────────────────────────────────────────────────────────────────────────────────────────┘│
│┌oui-table__body [tbody]──────────────────────────────────────────────────────────────────────┐│
││┌oui-table__row [tr]────────────────────────────────────────────────────────────────────────┐││
│││┌oui-table__cell [td]────────┐┌oui-table__cell [td]─────────┐┌oui-table__cell [td]────────┐│││
││││                            ││                             ││                            ││││
││││                            ││                             ││                            ││││
││││                            ││                             ││                            ││││
│││└────────────────────────────┘└─────────────────────────────┘└────────────────────────────┘│││
││└───────────────────────────────────────────────────────────────────────────────────────────┘││
││┌oui-table__row [tr]────────────────────────────────────────────────────────────────────────┐││
│││┌oui-table__cell [td]────────┐┌oui-table__cell [td]─────────┐┌oui-table__cell [td]────────┐│││
││││                            ││                             ││                            ││││
││││                            ││                             ││                            ││││
││││                            ││                             ││                            ││││
│││└────────────────────────────┘└─────────────────────────────┘└────────────────────────────┘│││
││└───────────────────────────────────────────────────────────────────────────────────────────┘││
│└─────────────────────────────────────────────────────────────────────────────────────────────┘│
└───────────────────────────────────────────────────────────────────────────────────────────────┘
```

### Advanced CSS for oui-angular component

A fake header is added with flexbox based positionning.
This markup is automatically created with the AngularJS oui-table component.

```
┌ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ┐
│ oui-table-container           │───────────────────────────────────────────────────────────────┐
├ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ┘                                                               │
│┌oui-table-container__headers─────────────────────────────────────────────────────────────────┐│
││┌oui-table-container__header──┐┌oui-table-container__header──┐┌oui-table-container__header──┐││
│││                             ││                             ││                             │││
│││                             ││                             ││                             │││
│││                             ││                             ││                             │││
││└─────────────────────────────┘└─────────────────────────────┘└─────────────────────────────┘││
│└─────────────────────────────────────────────────────────────────────────────────────────────┘│
│┌oui-table-container__body────────────────────────────────────────────────────────────────────┐│
││┌oui-table [table]──────────────────────────────────────────────────────────────────────────┐││
│││                                                                                           │││
│││                                [use the oui-table markup]                                 │││
│││                                                                                           │││
││└───────────────────────────────────────────────────────────────────────────────────────────┘││
│└─────────────────────────────────────────────────────────────────────────────────────────────┘│
└───────────────────────────────────────────────────────────────────────────────────────────────┘
```

## Modifier

### .oui-table_responsive

By default, the table is not responsive. But if want it to be responsive, add `oui-table_responsive` class.

## Mixins

```less
  @import 'oui-table/_mixins';
```

### .table-base

Define the base styles for a table.

```less
#oui > .table-base();
```

```less
#oui > .table-base(
  @oui-table-width: Number,
  @oui-table-margin: Number
);
```

### .table-header

Define the base styles for the table headers.

```less
#oui > .table-header();
```

```less
#oui > .table-header(
  @oui-table-header-background-color: Color,
  @oui-table-header-font-color: Color
);
```

### .table-cell

Define the base styles for the table cells.

```less
#oui > .table-cell();
```

```less
#oui > .table-cell(
  @oui-table-cell-background-color: Color,
  @oui-table-cell-border-color: Color,
  @oui-table-cell-font-color: Color,
  @oui-table-cell-padding: Number
);
```

### .table-cell-sortable

Define the base styles for the sortable table cells.

```less
#oui > .table-cell-sortable();
```

```less
#oui > .table-cell-sortable(
  @oui-table-arrow-size: Number
);
```

### .table-arrow-asc

Define the base styles for the arrow asc.

```less
#oui > .table-arrow-asc();
```

```less
#oui > .table-arrow-asc(
  @oui-table-arrow-color: Color,
  @oui-table-arrow-size: Number
);
```
### .table-arrow-desc

Define the base styles for the arrow desc.

```less
#oui > .table-arrow-desc();
```

```less
#oui > .table-arrow-desc(
  @oui-table-arrow-color: Color,
  @oui-table-arrow-size: Number
);
```

### .table-container

Define the base styles for the wrapper that contains oui-table with a fixed header.

```less
#oui > .table-container();
```

### .table-responsive

Define additional styles to oui-table to make it responsive.

```less
#oui > .table-responsive();
```
