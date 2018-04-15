---
layout: default
---

# React image lazy loading
React image lazy loading component inspired by [Polymer's Iron Image](https://www.webcomponents.org/element/PolymerElements/iron-image)
```
npm i react-image-lazy-load-component
```

## How to use

1. **npm install react-image-lazy-load-component**
2. You will need 2 different images
    - First one will be the image you want to display once it's loaded. ( Image in full HD )
    - Second one will be a copy of the first image scaled down to **1%.** ( Image that will be displayed until the full HD image is loaded )
3. Your code should look something like this  :arrow_down:

```javascript
import React from 'react'; // Import react
import IronImage from 'react-image-lazy-load'; // Import our component

// Images
import image from './iron-image-small.jpg'; // Low quality image ( Scaled down to 1% of it's original size )
const hdUrl = 'https://images.unsplash.com/photo-1478562853135-c3c9e3ef7905'; // Full HD image


const App = () => (
  <div>
      <IronImage alt="Enter alt text" placeholder={image} src={hdUrl} />
  </div>
);

export default App;
```
### Congrats! You made it.

![alt Lazy load image preview](https://cdn-images-1.medium.com/max/800/1*st2DLLQ2Sx1fdj1bcwuROQ.gif)

If you want to start from scratch and create your own image lazy loading component check out our Medium [blog post](https://medium.com/jsguru/react-image-lazy-loading-component-246e0cdcce02)
