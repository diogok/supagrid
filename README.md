# Supagrid

A simple "supergrid" HTML5 table grid editor, with no other dependency and lightweight.

_EXPERIMENTAL_

[http://diogok.github.io/supagrid](Check it out).

## Usage

Include the CSS and JS:

    <link rel="stylesheet" href="supagrid.css" />
    <script src="supagrid.js" type="text/javascript"></script>

Create the container element:

    <div id='grid'></div>

Initiate the GRID:

    var fields = [];
    var data = [];

    var g = new Supagrid({
      element: document.getElementById('grid'),
      fields: fields,
      id_field: fields[0],
      data: data,
      on: {
        change: function(obj,field,value) {
        },
        focus: function(obj) {
        }
      }
    });


Supagrid automatically binds to the objects on the data element, so if an object changes the grid will update and if the grid changes it will update the object.
         
Soon it will also bind the the data array to check it items were added or removed.

You can optionally apply custom styles:


## License

MIT

