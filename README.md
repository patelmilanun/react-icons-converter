# @milu/react-icons-converter

SVG icon converter to format required for use with [react-icons](https://www.npmjs.com/package/react-icons) package.

The source code was taken from [react-icons/logics.js](https://github.com/react-icons/react-icons/blob/master/packages/react-icons/scripts/logics.ts) file and modified. The package name inspired by [react-icons-converter](https://github.com/matthova/react-icons-converter.sh).

¯\\_(ツ)_/¯

### Installation

-   `npm i @milu/react-icons-converter`

### Usage example

```js
import { GenIcon } from 'react-icons';
import { createIconTreeFromSVG } from '@milu/react-icons-converter';

const SVGSource = ` /* here will be the source code of your svg icon */ `;

const IconTree = createIconTreeFromSVG(SVGSource);

export const Icon = GenIcon(IconTree);
```

### See also

-   [react-icons-lib-only](https://github.com/e965/react-icons-lib-only)

### Note

This is a fork of original library [react-icons-converter](https://github.com/e965/react-icons-converter). The original library is no longer maintained and since it's last update there were new vulnerabilities. So I decided to fork it and fix it. There were some breaking changes in 1 library(fast-xml-parser) after upgrade, which was also taken care of in this modified fork.
