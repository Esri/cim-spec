# Point symbol of a pin
A simple pin defined as a CIMPointSymbol with a single CIMVectorMarker layer.

Appearance: ![Image of pin symbol](/images/pin.png)

JSON:
```
{
	"type": "CIMPointSymbol",
	"symbolLayers": [{
		"type": "CIMVectorMarker",
		"enable": true,
		"anchorPoint": {
			"x": 0,
			"y": -0.5
		},
		"anchorPointUnits": "Relative",
		"dominantSizeAxis3D": "Y",
		"size": 14,
		"billboardMode3D": "FaceNearPlane",
		"frame": {
			"xmin": 0.0,
			"ymin": 0.0,
			"xmax": 17.0,
			"ymax": 17.0
		},
		"markerGraphics": [{
			"type": "CIMMarkerGraphic",
			"geometry": {
				"curveRings": [[[13.08,
				13.55],
				{
					"b": [[13.08,
					13.54],
					[13.08,
					13.54],
					[13.08,
					13.54]]
				},
				[13.08,
				4.52],
				[8.5,
				0.0],
				[3.92,
				4.51],
				[3.92,
				13.55],
				[3.92,
				13.55],
				{
					"b": [[8.5,
					17.0],
					[3.92,
					16.04],
					[5.97,
					17.0]]
				},
				{
					"b": [[13.08,
					13.55],
					[11.03,
					17.0],
					[13.08,
					16.04]]
				}]]
			},
			"symbol": {
				"type": "CIMPolygonSymbol",
				"symbolLayers": [{
					"type": "CIMSolidStroke",
					"enable": true,
					"capStyle": "Round",
					"joinStyle": "Round",
					"lineStyle3D": "Strip",
					"miterLimit": 10,
					"width": 0,
					"color": {
						"type": "CIMRGBColor",
						"values": [110,
						110,
						110,
						100]
					}
				},
				{
					"type": "CIMSolidFill",
					"enable": true,
					"color": {
						"type": "CIMRGBColor",
						"values": [0,
						122,
						194,
						100]
					}
				}]
			}
		}],
		"scaleSymbolsProportionally": true,
		"respectFrame": true
	}],
	"haloSize": 1,
	"scaleX": 1,
	"angleAlignment": "Display"
}
```

# Point symbol of a campground
A simple pin defined as a CIMPointSymbol with two CIMVectorMarker layers. The white circle is a CIMVectorMarker with a white CIMSolidFill and a gray CIMSolidStroke. The green tent is a CIMVectorMarker with a green CIMSolidFill.

Appearance: ![Image of campground symbol](/images/campground.png)

JSON:
```
{
	"type": "CIMPointSymbol",
	"symbolLayers": [{
		"type": "CIMVectorMarker",
		"enable": true,
		"anchorPoint": {
			"x": 0,
			"y": 0
		},
		"anchorPointUnits": "Relative",
		"dominantSizeAxis3D": "Y",
		"size": 15.75,
		"billboardMode3D": "FaceNearPlane",
		"frame": {
			"xmin": 0.0,
			"ymin": 0.0,
			"xmax": 21.0,
			"ymax": 21.0
		},
		"markerGraphics": [{
			"type": "CIMMarkerGraphic",
			"geometry": {
				"rings": [[[10.51,
				12.96],
				[8.63,
				4.02],
				[2.0,
				4.02],
				[10.5,
				18.0],
				[19.0,
				4.02],
				[12.4,
				4.02],
				[10.51,
				12.96]]]
			},
			"symbol": {
				"type": "CIMPolygonSymbol",
				"symbolLayers": [{
					"type": "CIMSolidStroke",
					"enable": true,
					"capStyle": "Round",
					"joinStyle": "Round",
					"lineStyle3D": "Strip",
					"miterLimit": 10,
					"width": 0,
					"color": {
						"type": "CIMRGBColor",
						"values": [0,
						0,
						0,
						100]
					}
				},
				{
					"type": "CIMSolidFill",
					"enable": true,
					"color": {
						"type": "CIMRGBColor",
						"values": [113,
						201,
						110,
						100]
					}
				}]
			}
		}],
		"scaleSymbolsProportionally": true,
		"respectFrame": true
	},
	{
		"type": "CIMVectorMarker",
		"enable": true,
		"colorLocked": true,
		"anchorPointUnits": "Relative",
		"dominantSizeAxis3D": "Y",
		"size": 18.5,
		"billboardMode3D": "FaceNearPlane",
		"frame": {
			"xmin": -5.0,
			"ymin": -5.0,
			"xmax": 5.0,
			"ymax": 5.0
		},
		"markerGraphics": [{
			"type": "CIMMarkerGraphic",
			"geometry": {
				"curveRings": [[[0.0,
				5.0],
				{
					"a": [[0.0,
					5.0],
					[0.0,
					0.0],
					0,
					1]
				},
				[0.0,
				5.0]]]
			},
			"symbol": {
				"type": "CIMPolygonSymbol",
				"symbolLayers": [{
					"type": "CIMSolidStroke",
					"enable": true,
					"capStyle": "Round",
					"joinStyle": "Round",
					"lineStyle3D": "Strip",
					"miterLimit": 10,
					"width": 0.5,
					"color": {
						"type": "CIMRGBColor",
						"values": [167,
						169,
						172,
						100]
					}
				},
				{
					"type": "CIMSolidFill",
					"enable": true,
					"color": {
						"type": "CIMRGBColor",
						"values": [255,
						255,
						255,
						100]
					}
				}]
			}
		}],
		"scaleSymbolsProportionally": true,
		"respectFrame": true
	}],
	"haloSize": 1,
	"scaleX": 1,
	"angleAlignment": "Display"
}
```
# Point symbol of a highway shield
A simple pin defined as a CIMPointSymbol with two CIMVectorMarker layers. The blue portion of the shield is a CIMVectorMarker with a blue CIMSolidFill and a white CIMSolidStroke. The red crown of the shield is a CIMVectorMarker with a red fill and a white CIMSolidStroke.

Appearance: ![Image of a highway shield](/images/highwayShield.png)

JSON:
```
{
	"type": "CIMPointSymbol",
	"symbolLayers": [{
		"type": "CIMVectorMarker",
		"enable": true,
		"colorLocked": true,
		"anchorPoint": {
			"x": 0,
			"y": -0.5
		},
		"anchorPointUnits": "Relative",
		"dominantSizeAxis3D": "Y",
		"size": 15.75,
		"billboardMode3D": "FaceNearPlane",
		"frame": {
			"xmin": 0.0,
			"ymin": 0.0,
			"xmax": 17.0,
			"ymax": 17.0
		},
		"markerGraphics": [{
			"type": "CIMMarkerGraphic",
			"geometry": {
				"curveRings": [[[17.0,
				6.0],
				[0.0,
				6.0],
				{
					"b": [[0.25,
					8.0],
					[0.0,
					6.0],
					[0.04,
					7.32]]
				},
				{
					"b": [[1.26,
					10.51],
					[0.56,
					9.01],
					[1.26,
					10.51]]
				},
				{
					"b": [[5.0,
					8.8],
					[1.26,
					10.51],
					[3.04,
					8.8]]
				},
				{
					"b": [[8.5,
					11.0],
					[7.1,
					8.8],
					[8.5,
					11.0]]
				},
				{
					"b": [[12.0,
					8.85],
					[8.5,
					11.0],
					[10.0,
					8.85]]
				},
				{
					"b": [[15.75,
					10.5],
					[14.1,
					8.85],
					[15.75,
					10.5]]
				},
				{
					"b": [[16.75,
					8.0],
					[15.75,
					10.5],
					[16.39,
					9.17]]
				},
				{
					"b": [[17.0,
					6.0],
					[16.96,
					7.32],
					[17.0,
					6.0]]
				}]]
			},
			"symbol": {
				"type": "CIMPolygonSymbol",
				"symbolLayers": [{
					"type": "CIMSolidStroke",
					"enable": true,
					"capStyle": "Round",
					"joinStyle": "Round",
					"lineStyle3D": "Strip",
					"miterLimit": 10,
					"width": 0.25,
					"color": {
						"type": "CIMRGBColor",
						"values": [255,
						255,
						255,
						100]
					}
				},
				{
					"type": "CIMSolidFill",
					"enable": true,
					"color": {
						"type": "CIMRGBColor",
						"values": [175,
						30,
						45,
						100]
					}
				}]
			}
		}],
		"scaleSymbolsProportionally": true,
		"respectFrame": true
	},
	{
		"type": "CIMVectorMarker",
		"enable": true,
		"anchorPointUnits": "Relative",
		"dominantSizeAxis3D": "Y",
		"size": 15.75,
		"billboardMode3D": "FaceNearPlane",
		"frame": {
			"xmin": 0.0,
			"ymin": 0.0,
			"xmax": 17.0,
			"ymax": 17.0
		},
		"markerGraphics": [{
			"type": "CIMMarkerGraphic",
			"geometry": {
				"curveRings": [[[17.0,
				14.39],
				{
					"b": [[16.49,
					9.7],
					[17.0,
					14.39],
					[16.99,
					11.79]]
				},
				{
					"b": [[8.5,
					2.61],
					[15.12,
					4.31],
					[9.92,
					2.61]]
				},
				{
					"b": [[0.51,
					9.7],
					[6.74,
					2.61],
					[1.81,
					4.6]]
				},
				{
					"b": [[0.0,
					14.39],
					[0.01,
					11.79],
					[0.0,
					14.39]]
				},
				[17.0,
				14.39]]]
			},
			"symbol": {
				"type": "CIMPolygonSymbol",
				"symbolLayers": [{
					"type": "CIMSolidStroke",
					"enable": true,
					"capStyle": "Round",
					"joinStyle": "Round",
					"lineStyle3D": "Strip",
					"miterLimit": 10,
					"width": 0.25,
					"color": {
						"type": "CIMRGBColor",
						"values": [255,
						255,
						255,
						100]
					}
				},
				{
					"type": "CIMSolidFill",
					"enable": true,
					"color": {
						"type": "CIMRGBColor",
						"values": [0,
						63,
						135,
						100]
					}
				}]
			}
		}],
		"scaleSymbolsProportionally": true,
		"respectFrame": true
	}],
	"haloSize": 1,
	"scaleX": 1,
	"angleAlignment": "Display"
}

```
