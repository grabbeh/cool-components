# cool-components

A list of (really) basic React components that use [styled-system](https://github.com/jxnblk/styled-system) for styling. This repo mainly exists because I wanted to understand how React components could be made available through npm. Turns out it's not quite as simple as just including the base code! After some in-depth research (googling) I entered the murky world of Webpack, babel-loader and peerDependencies. 

After a few false starts (as is to be expected when you would rather copy and paste different strings of text which have no real meaning to you, than actually read the docs), the module is now installable through ```npm install cool-components``` and you can then require a range of components which support styling via ```styled-system``` with a full overview available at [docs.grabeh.net](https://docs.grabeh.net).

    import { Box, Theme, Checkbox, Input, Select, Tab, TabList, TabPanels, Tabs, Text } from 'cool-components'

Here's an example of what you can do, with the props passed to the component acting to style it accordingly, without having to worry about coding the specific CSS (as styled-system seamlessly takes care of all that in the background):

```
import { Box, Text } from 'cool-components'

<Box bg="blue" p={3} m={3}>
    <Text fontWeight="bold">
        Hello world
    </Text>
</Box>
```

In order to work, the module/styled-system needs a theme that defines various values (colors, spacing etc). It currently uses [Tachyons System](https://github.com/tachyons-css/tachyons-system) but I think this can be overridden if you use a separate theme provider.

If you want to use something like the above, you should definitely use [Rebass](https://rebassjs.org/)!
