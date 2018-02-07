# Jeux de données utilisés

## Données géographiques

Afin de représenter les différents départements de France métropolitaine, nous utilisons un fichier GeoJSON <a href="https://github.com/ArnaudBru/ProjetBAC/blob/master/data/departements.geojson">departements.geojson</a> obtenu via le GitHub de <a href="https://github.com/gregoiredavid">Gregoire David</a>.
Ce fichier contient chacun des départements de France Métropolitaine. Il est organisé de la façon suivante

	{
		"type":"FeatureCollection",
		"features":[{
			"type":"Feature",
			"geometry":{
				"type":"Polygon",
				"coordinates":[[[3.172704,50.011997],[3.182198,50.012336],[3.205139,50.01835],[3.24521,50.02812],[3.257914,50.024437],
				...
				,[3.002756,49.218836],[2.997742,49.223581],[2.986693,49.218745],[2.985455,49.213082],[2.990226,49.210675]]]
			},
			"properties":{
				"code":"02",
				"nom":"Aisne"
			}
		},
		{
			"type":"Feature",
			"geometry":{
				"type":"Polygon",
				"coordinates":[[[3.414789,48.390269],[3.416604,48.399073],[3.422079,48.413341],[3.419746,48.416486],[3.413623,48.41434],
				...
				,[3.433818,48.361626],[3.427509,48.359976],[3.423838,48.365144],[3.421681,48.371728],[3.413273,48.376301],[3.414789,48.390269]]]
			},
			"properties":{
				"code":"10",
        "nom":"Aube"
			}
		},

		...

	}
  
Chaque feature représente ici un département, elle contient notamment un polygone qui représente les contours du département stockés sous forme d'une liste de points. Pour chacun des départements, on trouve deux propriétés, le nom du département ainsi que son code.

Type du fichier: Fichier GEOJSON (.geojson)
Taille: 1,03 Mo
Source: <a href="https://github.com/gregoiredavid/france-geojson">France Geojson</a>

