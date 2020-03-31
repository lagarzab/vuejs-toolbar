# Toolbar
A simple toolbar component used to hold site navigation, logos, titles etc for your site.

## Usage
The toolbar component exports multiple components. The default export is the `toolbar` component.
You can also use the `toolbarButton` which already contains some default styling to work within the `toolbar` itself.

### `toolbar` Component
`toolbar` has 3 slots available for placement of your links, buttons, logos and text.
- `left`: flex item, 1/3 width, left aligned
- `middle`: flex item, 1/3 width, center aligned
- `right`: flex item, 1/3 width, right aligned

### `toolbarButton` Component
`toolbarButton` has one prop and one slot (default)
- `href`: default is `#`.
- `default` slot: use this to pass the label for your link/button.


Here is an example on how to use these components:
```
    <toolbar>
        <template #left>
            <img src='logo.png' />
        </template>
        <template #right>
            <toolbar-button href='/another.htm'>Button Name</toolbar-button>
        </template>
    </toolbar>
```
