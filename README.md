# guild-media-queries
* includes three screen sizes: (Portrait phones or greater, Portrait Tablets or greater, and Desktops or greater):
```js
import css from 'styled-jsx/css';
import { bps, } from '../../lib/styling/';

export default css`
/* Mobile Phones on Portrait or greater: */
body{
  background: orange
}

/* Landscape phones or greater (including tablets only portrait) */
@media (min-width: ${bps.small + 1}px){
  body{
    background: pink;
  }
}


/* Landscape Tablets or greater 
(including large tablets on portrait and desktop) */
@media (min-width: ${bps.large + 1}px){
  body{
    background: red;
  }
}

`;


// bps.small = 500;
// bps.medium = 800;
// bps.large = 1000;
// bps.huge = 1200;
```
