# Button
Buttons let users take actions and make choices with a single click or tap.

![Button components](https://make.wordpress.org/design/files/2019/03/button.png)

For design guidelines, visit [this doc](/packages/components/src/button/DESIGN.md).

### Usage

Renders a button with default style.

```jsx
import { Button } from "@wordpress/components";

const MyButton = () => (
	<Button isDefault>
		Click me!
	</Button>
);
```

### Props

The presence of a `href` prop determines whether an `anchor` element is rendered instead of a `button`.

Props not included in this set will be applied to the `a` or `button` element.

Name | Type | Default | Description
--- | --- | --- | ---
`disabled` | `bool` | `false` | Whether the button is disabled. If `true`, this will force a `button` element to be rendered.
`href` | `string` | `undefined` | If provided, renders `a` instead of `button`.
`isDefault` | `bool` | `false` | Renders a default button style.
`isPrimary` | `bool` | `false` | Renders a primary button style.
`isTertiary` | `bool` | `false` | Renders a text-based button style.
`isDestructive` | `bool` | `false` | Renders a red text-based button style to indicate destructive behavior.
`isLarge` | `bool` | `false` | Increases the size of the button.
`isSmall` | `bool` | `false` | Decreases the size of the button.
`isToggled` | `bool` | `false` | Renders a toggled button style.
`isBusy` | `bool` | `false` | Indicates activity while a action is being performed.
`isLink` | `bool` | `false` | Renders a button with an anchor style.
`focus` | `bool` | `false` | Whether the button is focused.

### Related components

- To group buttons together, use the `ButtonGroup` component.
- To display an icon inside the button, use the `IconButton` component.
