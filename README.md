Reactjs Component for Facebook like photo/image grids
=====================================================

This component shows images in a neat square (or whatever dimensions you want) grid. Acts like facebooks image grids. Switches between two modes randomly (small images on right or bottom).

The component tries to figure out the best image to show as the main image (based on their dimensions).

<a href='https://cdn.rawgit.com/mukeshsoni/react-photo-grid/master/example/index.html' target='_blank'>Live Demo</a>

![How it looks](https://farm8.staticflickr.com/7484/15736005117_57154548cc.jpg "How it looks")

#Usage
```
var imageData = [
            'http://lorempixel.com/400/400/',
            'http://lorempixel.com/500/700/',
            'http://lorempixel.com/600/500/',
            'http://lorempixel.com/600/800/'
    ];
var imageGrid = (
            <ReactPhotoGrid
                onImageClick={handleImageClick}
                data={imageData} />
            );
React.render(imageGrid, document.getElementById('container'));
```

You can also pass gridSize as a property. It's a string which consists of width and height separated by an x. E.g. gridSize="500x500".

If you don't pass any gridSize, the grid size is chosen based on the parent's width.
