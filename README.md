## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/Aichii1/curly-system/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Aichii1/curly-system/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.


<html>
<head>
  <title>A Leaflet map!</title>
  <link rel="stylesheet" href="http://cdn.leafletjs.com/leaflet-0.7.3/leaflet.css"/>
  <script src="http://cdn.leafletjs.com/leaflet-0.7.3/leaflet.js"></script>
  <script src="D:\Leaflet\js\leaflet.ajax.min.js"></script>
  <style>
    #map{ width: 900px; height: 500px; }
  </style>
</head>
<body>

  <div id="map"></div>

  <script>

  // initialize the map
  var map = L.map('map').setView([58.3934, 13.851], 15);
  var geojsonLayer = new L.GeoJSON.AJAX("stationer_s.geojson");       
geojsonLayer.addTo(map);

 

// load a tile layer

  L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
    }).addTo(map);
 
 //geojson 

 

  </script>
</body>
</html>


