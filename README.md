# COLINA CSS

Colina CSS is a CSS library **based on utilities**.
___
## Table of contents

- [Quick Install](#quick-install)
- [What's included](#whats-included)
- [Adding in Angular projects](#adding-in-angular-projects)
- [Adding in React projects](#adding-in-react-projects)
- [Documentation](#documentation)
- [Creator](#creator)

## Quick Install

- **npm**
```
npm i colina-css
```
## What's included 

Within the download, you will find the directory with a single minified style file. Kind of:

```
dist
    ├── css
        └── colina.min.css
```

## Adding in Angular projects
Adding Colina CSS to an angular project is as easy as just adding the **colina.min.css** to **angular.json** file.<br>
So, open angular.json file, inside of projects → project-name → architect → styles. Add a new item to it with the path for colina.min.css.
```
...
    "styles": [
        "node_modules/colina-css/dist/css/colina.min.css",
        "src/styles.css"
    ],
...
```
## Adding in React projects
Adding Colina CSS to a react project is as easy as adding the import from the **colina.min.css** file into **index.js** file. <br>
```
import ReactDom from 'react-dom';
import '../node_modules/colina-css/dist/css/colina.min.css'

ReactDom.render(<App />, document.querySelector('#root'));

```
## Documentation
These are the most relevant classes in the library
```
• Hover Animations:

hover_zoom ->  transform: scale(1.1); transition: 0.2s;

• Display:

none -> display: none
block -> display: block
hidden -> display: hidden
grid -> display: grid
inline_grid -> display: inline-grid
list_item -> display: list-item
contents -> display: contents
inline_block -> display: inline-block
inline -> display: inline
flex -> display: flex
inline_flex -> display: inline-flex
inline_table -> display: inline-table
table_caption -> display: table-caption
table_cell -> display: table-cell
table_column -> display: table-column
table_column_group -> display:  table-column-group
table_footer_group -> display: table-footer-group
table_header_group  -> display: table-header-group
table_row_group -> display:  table-row-group
table_row -> display: table-row
flow_root -> display:  flow-root

• Flexbox:

flex -> display: flex
flex_col -> flex-direction: column

- Align items
items_start -> align-items: flex-start
items_center -> align-items: center
items_baseline -> align-items: baseline
items_stretch -> align-items: stretch
items_end -> align-items: flex-end

- Align selft
self_auto -> align-self: auto
self_start -> align-self: start
self_end -> align-self: end
self_center -> align-self: center
self_stretch -> align-self: stretch

- Justify Content
justify_start -> justify-content: flex-start
justify_between -> justify-content: space-between
justify_center -> justify-content: center
justify_around -> justify-content: space-around
justify_evenly -> justify-content: space-evenly
justify_end -> justify-content: flex-end

- Justify Items
justify_items_start -> justify-items: start
justify_items_center -> justify-items: stretch
justify_items_strech -> justify-items: space-between
justify_items_end -> justify-items: end

- Flex Wrap
flex_wrap -> flex-wrap: wrap
flex_wrap_reverse -> flex-wrap: wrap
flex_nowrap -> flex-wrap: nowrap

• Gap:

gap_xs -> gap: 1rem
gap_sm -> gap: 1.5rem
gap_md -> gap: 2.5rem
gap_lg -> gap: 3.5rem

• Cursor:

cursor_auto -> cursor: auto
cursor_default -> cursor: default
cursor_pointer -> cursor: pointer
cursor_wait -> cursor: wait
cursor_text -> cursor: text
cursor_move -> cursor: move
cursor_help -> cursor: help
cursor_disabled -> cursor: not-allowed

• Font Size:

text_sx -> font-size: 0.75rem; line-height: 1rem
text_sm -> font-size: 0.875rem; line-height: 1.25rem
text_md -> font-size: 1rem; line-height: 1.5rem
text_lg -> font-size: 1.125rem; line-height: 1.75rem
text_xl -> font-size:  1.25rem; line-height:  1.75rem
text_2xl -> font-size: 1.5rem; line-height: 2rem
text_3xl -> font-size: 1.875rem; line-height: 2.25rem
text_4xl -> font-size: 2.25rem; line-height: 2.25rem

• Text Alignment

text_left -> text-align: left
text_center -> text-align: center
text_right -> text-align: right
text_justify -> text-align: justify

• Text Style

text_normal -> font-style: normal
initial -> font-style: initial
italic -> font-style: italic
oblique -> font-style: oblique

• Font weight

bold -> font-weight: bold
no_bold -> font-weight: normal
bold_400 -> font-weight: 400
bold_500 -> font-weight: 500
bold_600 -> font-weight: 600
bold_700 -> font-weight: 700

• Text Transform

uppercase -> text-transform: uppercase
lowercase -> text-transform: lowercase
capitalize -> text-transform: capitalize
normal_text -> text-transform: none
underline -> text-decoration: underline
no_underline -> text-decoration: none
line_through -> text-decoration: line-through

• Line Height
lh_sm -> line-height: 20px
lh_md -> line-height: 25px
lh_lg -> line-height: 30px

• Border

- Border Solid
border_none -> border: none
border_left -> border-left: 1.5px solid #e2e8f0
border_top -> border-top: 1.5px solid #e2e8f0
border_right -> border-right: 1.5px solid #e2e8f0
border_bottom -> border-bottom: 1.5px solid #e2e8f0
border_all -> border-all: 1.5px solid #e2e8f0

- Border Dotted
dotted_left -> border-left: 2px dotted lightgray
dotted_top -> border-top: 2px dotted lightgray
dotted_right -> border-right: 2px dotted lightgray
dotted_bottom -> border-bottom: 2px dotted lightgray
dotted_all -> border-all: 2px dotted lightgray

- Border Radius
rounded_none: border-radius: 0
rounded_sm: border-radius: 0.2rem
rounded_md: border-radius: 0.5rem
rounded_lg: border-radius: 1rem
rounded_circle: border-radius: 50%

• Box shadow

shadow_none -> box-shadow: none
shadow_sm -> box-shadow: 0 0.1rem 1rem rgba(0, 0, 0, 0.075)
shadow_md -> box-shadow: 0 0.1rem 1rem rgba(0, 0, 0, 0.15)
shadow_lg -> box-shadow: 0 0.1rem 1rem rgba(0, 0, 0, 0.3)
shadow_xl -> box-shadow: 0 0.1rem 1rem rgba(0, 0, 0, 0.5) 

• Positions

static -> position: static
fixed -> position: fixed
absolute -> position: absolute
relative -> position: relative 
sticky -> position: sticky 

• Overflow
overflow_auto -> overflow: auto
overflow_hidden -> overflow: hidden
overflow_visible -> overflow: scroll
overflow_y_visible -> overflow-y: scroll
overflow_y_hidden -> overflow-y: hidden
overflow_x_visible -> overflow-x: scroll
overflow_x_hidden -> overflow-x: hidden

• Visibility

visible -> visibility: visible 
invisible -> visibility: hidden 

• Positions

float_none -> float: none
float_left -> float: left
float_right -> float: right\

• Positions elements

top_0 -> 0px
right_0 -> 0px
bottom_0 -> 0px
left_0 -> 0px

inset_0 ->
    top: 0px;
    right: 0px;
    bottom: 0px;
    left: 0px;
inset_y_0 ->
    top: 0px;
    bottom: 0px;
inset_x_0 ->
    right: 0px;
    left: 0px;

• Layout

- Width:
w_0 -> width: 0
w_screen -> width: 100vh
w_auto -> width: auto
w_full -> width:  100%

- Height:
h0 -> height: 0
h_screen -> height: 100vh
h_auto -> height: auto
h_full -> height: 100%


• Outline

outline_none -> outline: none
outline_white -> outline: white
outline_black -> outline: black

• Z-Index

z_auto -> z-index: auto
z_10 -> z-index: 10
z_20 -> z-index: 20
z_30 -> z-index: 30
z_40 -> z-index: 40
z_50 -> z-index: 50


```

## Creator

**Ernesto Colina Jiménez**

- <https://github.com/ecolina05>
- <https://www.linkedin.com/in/ecolina05/>