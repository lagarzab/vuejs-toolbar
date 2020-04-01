# Toolbar
A simple toolbar component used to hold site navigation, logos, titles etc for your site.

## Usage
The toolbar component exports multiple components. The default export is the `toolbar` component.
You can also use the `toolbarButton` which already contains some default styling to work within the `toolbar` itself.

### `toolbarHeader` Component
`toolbarHeader` has 3 slots available for placement of your links, buttons, logos and text.
- `left`: flex item, 1/3 width, left aligned
- `middle`: flex item, 1/3 width, center aligned
- `right`: flex item, 1/3 width, right aligned

### `toolbarFooter` Component
`toolbarFooter` has two props and two slots available for placement of your links, buttons, logos and text.
- `legal` slot: flex item, 100% width, center aligned
- `contact` slot: flex item, 100% width, center aligned
- `hideLegalSection` prop: default false, when passed (as true) will hide the legal section of the footer.
- `hideContactSection` prop: default false, when passed (as true) will hide the contact section of the footer.


### `toolbarButton` Component
This is styled appear like a button.

`toolbarButton` has one prop and one slot (default).
- `href`: default is `#`.
- `default` slot: use this to pass the label for your link/button.

### `toolbarLink` Component
The only styling change from a regular link is the removal of text-decoration.

`toolbarLink` has one prop and one slot (default)
- `href`: default is `#`.
- `default` slot: use this to pass the label for your link/button.

### Note:
The difference between a link and button is that a button is styled to look more like a button larger button.  A link is pretty


Here is an example on how to use these components:
```
    <toolbar-header>
        <template #left>
            <img src='logo.png' />
        </template>
        <template #right>
            <toolbar-link href='/a-link-to-page.htm'>Button Name</toolbar-link>
            <toolbar-button href='/another.htm'>Button Name</toolbar-button>
        </template>
    </toolbar-header>
```
