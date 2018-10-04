# cool-components

A list of (really) basic React components. This repo mainly exists because I wanted to understand how React components could be made available through npm. Turns out it's not quite as simple as just including the base code! After some in-depth research (googling) I entered the murky world of Webpack, babel-loader and peerDependencies. 

After a few false starts (as is to be expected when you would rather copy and paste different strings of text which have no real meaning to you, than actually read the docs), the module is now installable through ```npm install cool-components``` and you can then require a range of components which support styling via ```styled-system``` with a full overview available at [docs.grabeh.net](https://docs.grabeh.net).

    import { Box, Theme, Checkbox, Input, Select, Tab, TabList, TabPanels, Tabs, Text } from 'cool-components'



