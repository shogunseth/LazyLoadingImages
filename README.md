# LazyLoadingImages
load low res image on initial page load to avoid render blocking and load high res image asyncronously 

load the js into the webpage: 
> <script src="lazyimage.js"></script> 

src attribute gets the low res version of the image, the onload is set to the lazyLoadFullRes function the parameters are the event itself and the full res image location: 
> <img src='lowresmin.jpeg' onload="lazyLoadFullRes(event,'highres.jpeg')" /> 
