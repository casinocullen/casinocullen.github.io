<head>
   <title>Places Traveled</title>
   <link rel = "stylesheet" href = "/assets/css/leaflet.css"/>
   <script src = "/assets/js/leaflet.js"></script>
   <script src="/assets/js/leaflet-providers.js"></script>
   <link rel="stylesheet" href="./assets/css/style.css">

</head>

<body>

   <!-- Title -->
   <div class="title">
         <div>
            <h1>Places traveled in North America<br>
            <span>and the journey continues...</span></h1>
         </div>
   </div>

   <!-- Map -->
   <div id = "map" style = "width: 99%; height:450px"></div>
   <script>
      // Creating map options
      var mapOptions = {
         center: [35.8283, -95.5795],
         zoom: 3.6
      }
      // Creating a map object
      var map = new L.map('map', mapOptions);
      
      // Creating a Layer object and adding layer to the map
      L.tileLayer.provider('USGS.USTopo').addTo(map);


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



      // Creating a marker
      var marker1 = L.marker([29.770, -95.390], markerOptions).addTo(map); //houston
      var marker2 = L.marker([40.670, -73.940], markerOptions).addTo(map); //New york
      var marker3 = L.marker([34.110, -118.410], markerOptions).addTo(map); //Los angeles
      var marker4 = L.marker([41.840, -87.680], markerOptions).addTo(map); //Chicago
      var marker5 = L.marker([40.010, -75.130], markerOptions).addTo(map); //Philadelphia
      var marker6 = L.marker([29.460, -98.510], markerOptions).addTo(map); //San antonio
      var marker7 = L.marker([37.770, -122.450], markerOptions).addTo(map); //San francisco
      var marker8 = L.marker([39.990, -82.990], markerOptions).addTo(map); //Columbus
      var marker9 = L.marker([30.310, -97.750], markerOptions).addTo(map); //Austin
      var marker10 = L.marker([35.110, -90.010], markerOptions).addTo(map); //Memphis
      var marker11 = L.marker([39.300, -76.610], markerOptions).addTo(map); //Baltimore
      var marker12 = L.marker([31.850, -106.440], markerOptions).addTo(map); //El paso
      var marker13 = L.marker([35.200, -80.830], markerOptions).addTo(map); //Charlotte
      var marker14 = L.marker([42.340, -71.020], markerOptions).addTo(map); //Boston
      var marker15 = L.marker([38.910, -77.020], markerOptions).addTo(map); //Washington
      var marker16 = L.marker([36.170, -86.780], markerOptions).addTo(map); //Nashville
      var marker17 = L.marker([36.210, -115.220], markerOptions).addTo(map); //Las vegas
      var marker18 = L.marker([35.470, -97.510], markerOptions).addTo(map); //Oklahoma city
      var marker19 = L.marker([30.070, -89.930], markerOptions).addTo(map); //New orleans
      var marker20 = L.marker([25.780, -80.210], markerOptions).addTo(map); //Miami
      var marker21 = L.marker([38.640, -90.240], markerOptions).addTo(map); //Saint louis
      var marker22 = L.marker([40.440, -79.980], markerOptions).addTo(map); //Pittsburgh
      var marker23 = L.marker([28.500, -81.370], markerOptions).addTo(map); //Orlando
      var marker24 = L.marker([35.820, -78.660], markerOptions).addTo(map); //Raleigh
      var marker25 = L.marker([34.720, -92.350], markerOptions).addTo(map); //Little rock
      var marker26 = L.marker([40.780, -111.930], markerOptions).addTo(map); //Salt lake city
      var marker27 = L.marker([35.970, -83.950], markerOptions).addTo(map); //Knoxville
      var marker28 = L.marker([41.310, -72.920], markerOptions).addTo(map); //New haven
      var marker29 = L.marker([43.7022, -72.2896], markerOptions).addTo(map); //Hanover
      var marker30 = L.marker([41.820, -71.420], markerOptions).addTo(map); //Providence
      var marker31 = L.marker([33.760, -84.420], markerOptions).addTo(map); //Atlanta
      var marker32 = L.marker([39.780, -86.150], markerOptions).addTo(map); //Indianapolis
      var marker33 = L.marker([44.4759, -73.2121], markerOptions).addTo(map); //Burlington
      var marker34 = L.marker([32.7767, -96.7970], markerOptions).addTo(map); //Dallas
      var marker35 = L.marker([32.0809, -81.0912], markerOptions).addTo(map); //Savannah
      var marker36 = L.marker([43.6591, -70.2568], markerOptions).addTo(map); //Portland
      var marker37 = L.marker([43.0481, -76.1474], markerOptions).addTo(map); //Syracuse
      var marker38 = L.marker([43.0962, -79.0377], markerOptions).addTo(map); //Niagara Falls
      var marker39 = L.marker([43.6532, -79.3832], markerOptions).addTo(map); //Toronto
      var marker40 = L.marker([45.5019, -73.5674], markerOptions).addTo(map); //Montreal
      var marker41 = L.marker([46.8131, -71.2075], markerOptions).addTo(map); //Québec City
      var marker42 = L.marker([45.4215, -75.6972], markerOptions).addTo(map); //Ottawa
      var marker43 = L.marker([19.4326, -99.1332], markerOptions).addTo(map); //Mexico City
      var marker44 = L.marker([21.1619, -86.8515], markerOptions).addTo(map); //Cancun
      var marker45 = L.marker([42.9956, -71.4548], markerOptions).addTo(map); //Manchester
      var marker46 = L.marker([33.9519, -83.3576], markerOptions).addTo(map); //Athens
      var marker47 = L.marker([24.5551, -81.7800], markerOptions).addTo(map); //Key West
      var marker48 = L.marker([33.5186, -86.8104], markerOptions).addTo(map); //Birmingham
      var marker49 = L.marker([37.2090, -93.2923], markerOptions).addTo(map); //Springfield

      var popupContent1 = '<a>Houston TX<br>Home sweet home<br><img src="./../assets/travel_img/home.jpg"></a>';
      var popupContent2 = '<a>New York NY<br><img src="./../assets/travel_img/ny.jpeg"></a>';
      var popupContent3 = '<a>Los Angeles CA<br><img src="./../assets/travel_img/la.jpeg"></a>';
      var popupContent4 = '<a>Chicago IL<br><img src="./../assets/travel_img/la.jpeg"></a>';
      var popupContent5 = '<a>Philadelphia IL<br><img src="./../assets/travel_img/la.jpeg"></a>';
      var popupContent6 = '<a>San antonio TX<br><img src="./../assets/travel_img/sa.jpeg"></a>';
      var popupContent7 = '<a>San Francisco CA<br><img src="./../assets/travel_img/sf.jpeg"></a>';
      var popupContent8 = '<a>Columbus OH<br><img src="./../assets/travel_img/columbus.jpeg"></a>';
      var popupContent9 = '<a>Austin TX<br><img src="./../assets/travel_img/austin.jpg"></a>';
      var popupContent10 = '<a>Memphis TN<br><img src="./../assets/travel_img/memphis.jpeg"></a>';

      // Adding pop-up to the marker
      marker1.bindPopup(popupContent1, {maxWidth: "auto"});
      marker2.bindPopup(popupContent2, {maxWidth: "auto"});
      marker3.bindPopup(popupContent3, {maxWidth: "auto"});
      marker4.bindPopup(popupContent4, {maxWidth: "auto"});
      marker5.bindPopup(popupContent5, {maxWidth: "auto"});
      marker6.bindPopup(popupContent6, {maxWidth: "auto"});
      marker7.bindPopup(popupContent7, {maxWidth: "auto"});
      marker8.bindPopup(popupContent8, {maxWidth: "auto"});
      marker9.bindPopup(popupContent9, {maxWidth: "auto"});
      marker10.bindPopup(popupContent10, {maxWidth: "auto"});

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
