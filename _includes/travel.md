
<h2 id="travel" style="margin: 2px 0px 15px;">Travel</h2>

   <head>
      <title>Places Traveled</title>
      <link rel = "stylesheet" href = "/assets/css/leaflet.css"/>
      <script src = "/assets/js/leaflet.js"></script>
      <script src="http://unpkg.com/leaflet@latest/dist/leaflet.js"></script>
      <script src="/assets/js/leaflet-providers.js"></script>

   </head>

   <body>
      <div id = "map" style = "width:900px; height:580px"></div>
      <script>
         // Creating map options
         var mapOptions = {
            center: [39.8283, -98.5795],
            zoom: 4
         }
         // Creating a map object
         var map = new L.map('map', mapOptions);
         
         // Creating a Layer object
            var layer = L.tileLayer('https://tiles.stadiamaps.com/tiles/alidade_smooth_dark/{z}/{x}/{y}{r}.{ext}', {
                minZoom: 0,
                maxZoom: 20,
                attribution: '&copy; <a href="https://www.stadiamaps.com/" target="_blank">Stadia Maps</a> &copy; <a href="https://openmaptiles.org/" target="_blank">OpenMapTiles</a> &copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors',
                ext: 'png'
            });

        
         // Icon options
         var iconOptionsVisted = {
            iconUrl: './assets/img/map_icon.png',
            iconSize: [10, 12]
         }

         var iconOptionsNP = {
            iconUrl: './assets/img/np_icon.png',
            iconSize: [10, 12]
         }

         // Creating a custom icon
         var visitIcon = L.icon(iconOptionsVisted);
         var npIcon = L.icon(iconOptionsNP);

         // Creating Marker Options
         var markerOptions = {
            title: "MyLocation",
            clickable: true,
            icon: visitIcon
         }

         var npOptions = {
            title: "MyLocation",
            clickable: true,
            icon: npIcon
         }


         // Adding layer to the map
         map.addLayer(layer);
         
         // Creating a marker
         var marker1 = L.marker([29.770, -95.390], markerOptions); //houston
         var marker2 = L.marker([40.670, -73.940], markerOptions); //New york
         var marker3 = L.marker([34.110, -118.410], markerOptions); //Los angeles
         var marker4 = L.marker([41.840, -87.680], markerOptions); //Chicago
         var marker5 = L.marker([40.010, -75.130], markerOptions); //Philadelphia
         var marker6 = L.marker([29.460, -98.510], markerOptions); //San antonio
         var marker7 = L.marker([37.770, -122.450], markerOptions); //San francisco
         var marker8 = L.marker([39.990, -82.990], markerOptions); //Columbus
         var marker9 = L.marker([30.310, -97.750], markerOptions); //Austin
         var marker10 = L.marker([35.110, -90.010], markerOptions); //Memphis
         var marker11 = L.marker([39.300, -76.610], markerOptions); //Baltimore
         var marker12 = L.marker([31.850, -106.440], markerOptions); //El paso
         var marker13 = L.marker([35.200, -80.830], markerOptions); //Charlotte
         var marker14 = L.marker([42.340, -71.020], markerOptions); //Boston
         var marker15 = L.marker([38.910, -77.020], markerOptions); //Washington
         var marker16 = L.marker([36.170, -86.780], markerOptions); //Nashville
         var marker17 = L.marker([36.210, -115.220], markerOptions); //Las vegas
         var marker18 = L.marker([35.470, -97.510], markerOptions); //Oklahoma city
         var marker19 = L.marker([30.070, -89.930], markerOptions); //New orleans
         var marker20 = L.marker([25.780, -80.210], markerOptions); //Miami
         var marker21 = L.marker([38.640, -90.240], markerOptions); //Saint louis
         var marker22 = L.marker([40.440, -79.980], markerOptions); //Pittsburgh
         var marker23 = L.marker([28.500, -81.370], markerOptions); //Orlando
         var marker24 = L.marker([35.820, -78.660], markerOptions); //Raleigh
         var marker25 = L.marker([34.720, -92.350], markerOptions); //Little rock
         var marker26 = L.marker([40.780, -111.930], markerOptions); //Salt lake city
         var marker27 = L.marker([35.970, -83.950], markerOptions); //Knoxville
         var marker28 = L.marker([41.310, -72.920], markerOptions); //New haven
         var marker29 = L.marker([43.7022, -72.2896], markerOptions); //Hanover
         var marker30 = L.marker([41.820, -71.420], markerOptions); //Providence
         var marker31 = L.marker([33.760, -84.420], markerOptions); //Atlanta
         var marker32 = L.marker([39.780, -86.150], markerOptions); //Indianapolis
         var marker33 = L.marker([44.4759, -73.2121], markerOptions); //Burlington
         var marker34 = L.marker([32.7767, -96.7970], markerOptions); //Dallas
         var marker35 = L.marker([32.0809, -81.0912], markerOptions); //Savannah
         var marker36 = L.marker([43.6591, -70.2568], markerOptions); //Portland
         var marker37 = L.marker([43.0481, -76.1474], markerOptions); //Syracuse
         var marker38 = L.marker([43.0962, -79.0377], markerOptions); //Niagara Falls
         var marker39 = L.marker([43.6532, -79.3832], markerOptions); //Toronto
         var marker40 = L.marker([45.5019, -73.5674], markerOptions); //Montreal
         var marker41 = L.marker([46.8131, -71.2075], markerOptions); //Québec City
         var marker42 = L.marker([45.4215, -75.6972], markerOptions); //Ottawa
         var marker43 = L.marker([19.4326, -99.1332], markerOptions); //Mexico City
         var marker44 = L.marker([21.1619, -86.8515], markerOptions); //Cancun
         var marker45 = L.marker([42.9956, -71.4548], markerOptions); //Manchester
         var marker46 = L.marker([33.9519, -83.3576], markerOptions); //Athens
         var marker47 = L.marker([24.5551, -81.7800], markerOptions); //Key West
         var marker48 = L.marker([33.5186, -86.8104], markerOptions); //Birmingham
         var marker49 = L.marker([37.2090, -93.2923], markerOptions); //Springfield


         // Adding marker to the map
         marker1.addTo(map);
         marker2.addTo(map);
         marker3.addTo(map);
         marker4.addTo(map);
         marker5.addTo(map);
         marker6.addTo(map);
         marker7.addTo(map);
         marker8.addTo(map);
         marker9.addTo(map);
         marker10.addTo(map);
         marker11.addTo(map);
         marker12.addTo(map);
         marker13.addTo(map);
         marker14.addTo(map);
         marker15.addTo(map);
         marker16.addTo(map);
         marker17.addTo(map);
         marker18.addTo(map);
         marker19.addTo(map);
         marker20.addTo(map);
         marker21.addTo(map);
         marker22.addTo(map);
         marker23.addTo(map);
         marker24.addTo(map);
         marker25.addTo(map);
         marker26.addTo(map);
         marker27.addTo(map);
         marker28.addTo(map);
         marker29.addTo(map);
         marker30.addTo(map);
         marker31.addTo(map);
         marker32.addTo(map);
         marker33.addTo(map);
         marker34.addTo(map);
         marker35.addTo(map);
         marker36.addTo(map);
         marker37.addTo(map);
         marker38.addTo(map);
         marker39.addTo(map);
         marker40.addTo(map);
         marker41.addTo(map);
         marker42.addTo(map);
         marker43.addTo(map);
         marker44.addTo(map);
         marker45.addTo(map);
         marker46.addTo(map);
         marker47.addTo(map);
         marker48.addTo(map);
         marker49.addTo(map);

         // Adding pop-up to the marker
        marker1.bindPopup('Home');

         // Creating NP markers
         var np1 = L.marker([44.35, -68.21], npOptions); //Acadia
         var np2 = L.marker([29.25, -103.25], npOptions); //Big Bend
         var np3 = L.marker([25.65, -80.08], npOptions); //Biscayne
         var np4 = L.marker([37.57, -112.18], npOptions); //Bryce Canyon
         var np5 = L.marker([32.17, -104.44], npOptions); //Carlsbad Caverns
         var np6 = L.marker([36.24, -116.82], npOptions); //Death Valley
         var np7 = L.marker([25.32, -80.93], npOptions); //Everglades
         var np8 = L.marker([38.63, -90.19], npOptions); //Gateway Arch
         var np9 = L.marker([36.06, -112.14], npOptions); //Grand Canyon
         var np10 = L.marker([43.73, -110.8], npOptions); //Grand Teton
         var np11 = L.marker([35.68, -83.53], npOptions); //Great Smoky Mountains
         var np12 = L.marker([31.92, -104.87], npOptions); //Guadalupe Mountains
         var np13 = L.marker([19.38, -155.2], npOptions); //Hawaiʻi Volcanoes
         var np14 = L.marker([38.53, -78.35], npOptions); //Shenandoah
         var np15 = L.marker([44.6, -110.5], npOptions); //Yellowstone
         var np16 = L.marker([37.83, -119.5], npOptions); //Yosemite

         // Adding NP to the map
         np1.addTo(map);
         np2.addTo(map);
         np3.addTo(map);
         np4.addTo(map);
         np5.addTo(map);
         np6.addTo(map);
         np7.addTo(map);
         np8.addTo(map);
         np9.addTo(map);
         np10.addTo(map);
         np11.addTo(map);
         np12.addTo(map);
         np13.addTo(map);
         np14.addTo(map);
         np15.addTo(map);
         np16.addTo(map);

      </script>
   </body>
