# CSS Color API

## Endpoints:

## Random Color

### `randomcolor`

**GET** _gets a random color_

**Example:** `https://fun-fun-colors.herokuapp.com/randomcolor`


**NOTE** Please use the proper headers. This will work:
`headers: {
	'Accept': 'application/json',
	'Content-Type': 'application/json'
}`

#### Sample Response 

#### Success

	{
		color: 'plum',
		status: 200
	}

#### Fail

	{
		error: 'Error message',
		status: 500
	}

## Color by Name

### `colorcheck`

**GET** _gets a specific color from the list_

**NOTE** Please use the proper headers. This will work:
`headers: {
	'Accept': 'application/json',
	'Content-Type': 'application/json'
}`

This will return a color from the CSS Colors. The list is in alphabetical order. The possible numbers range from **0 to 146**


Params | Value | Description | Valid format example
------ | ---- | ------ | ------
`q` | string | `the color or part of the color to return the index of` | 22


**Example:** `https://fun-fun-colors.herokuapp.com/colorcheck?q=dark` || `https://fun-fun-colors.herokuapp.com/colorcheck?q=darkcyan`


#### Success

	{
		colorIndex: 22,
		status: 200
	}

#### Fail

	{
		error: 'Error message',
		status: 500
	}

## Color by id

### `color/:id`

**GET** _gets a specific color from the list_

**NOTE** Please use the proper headers. This will work:
`headers: {
	'Accept': 'application/json',
	'Content-Type': 'application/json'
}`

This will return a color from the CSS Colors. The list is in alphabetical order. The possible numbers range from **0 to 146**


Params | Value | Description | Valid format example
------ | ---- | ------ | ------
`id` | number | `the id/index of the color to return` | 22


**Example:** `https://fun-fun-colors.herokuapp.com/color/22`


#### Success

	{
		color: 'darkcyan',
		status: 200
	}

#### Fail

	{
		error: 'Error message',
		status: 500
	}



## All Colors

### `allcolors`

**GET** _gets an array of all colors_

**NOTE** Please use the proper headers. This will work:
`headers: {
	'Accept': 'application/json',
	'Content-Type': 'application/json'
}`

This will return an array of all CSS colors. The list is in alphabetical order.



**Example:** `https://fun-fun-colors.herokuapp.com/allcolors`


#### Success

	{
		status: 200,
		color: [
			"#f0f8ff",
			"#faebd7",
			"#00ffff",
			"#7fffd4",
			"#f0ffff",
			"#f5f5dc",
			"#ffe4c4",
			"#000000",
			"#ffebcd",
			"#0000ff",
			"#8a2be2",
			"#a52a2a",
			"#deb887",
			"#5f9ea0",
			"#7fff00",
			"#d2691e",
			"#ff7f50",
			"#6495ed",
			"#fff8dc",
			"#dc143c",
			"#00ffff",
			"#00008b",
			"#008b8b",
			"#b8860b",
			"#a9a9a9",
			"#a9a9a9",
			"#006400",
			"#bdb76b",
			"#8b008b",
			"#556b2f",
			"#ff8c00",
			"#9932cc",
			"#8b0000",
			"#e9967a",
			"#8fbc8f",
			"#483d8b",
			"#2f4f4f",
			"#00ced1",
			"#9400d3",
			"#ff1493",
			"#00bfff",
			"#696969",
			"#1e90ff",
			"#b22222",
			"#fffaf0",
			"#228b22",
			"#ff00ff",
			"#dcdcdc",
			"#f8f8ff",
			"#ffd700",
			"#daa520",
			"#808080",
			"#008000",
			"#adff2f",
			"#f0fff0",
			"#ff69b4",
			"#cd5c5c",
			"#4b0082",
			"#fffff0",
			"#f0e68c",
			"#e6e6fa",
			"#fff0f5",
			"#7cfc00",
			"#fffacd",
			"#add8e6",
			"#f08080",
			"#e0ffff",
			"#fafad2",
			"#d3d3d3",
			"#90ee90",
			"#ffb6c1",
			"#ffa07a",
			"#20b2aa",
			"#87cefa",
			"#778899",
			"#b0c4de",
			"#ffffe0",
			"#00ff00",
			"#32cd32",
			"#faf0e6",
			"#800000",
			"#66cdaa",
			"#0000cd",
			"#ba55d3",
			"#9370db",
			"#3cb371",
			"#7b68ee",
			"#00fa9a",
			"#48d1cc",
			"#c71585",
			"#191970",
			"#f5fffa",
			"#ffe4e1",
			"#ffdead",
			"#000080",
			"#fdf5e6",
			"#808000",
			"#6b8e23",
			"#ffa500",
			"#ff4500",
			"#da70d6",
			"#eee8aa",
			"#98fb98",
			"#afeeee",
			"#db7093",
			"#ffefd5",
			"#ffdab9",
			"#cd853f",
			"#ffc0cb",
			"#dda0dd",
			"#b0e0e6",
			"#800080",
			"#ff0000",
			"#bc8f8f",
			"#4169e1",
			"#8b4513",
			"#fa8072",
			"#f4a460",
			"#2e8b57",
			"#fff5ee",
			"#a0522d",
			"#c0c0c0",
			"#87ceeb",
			"#6a5acd",
			"#708090",
			"#708090",
			"fffafa",
			"#00ff7f",
			"#4682b4",
			"#d2b48c",
			"#008080",
			"#d8bfd8",
			"#ff6347",
			"#40e0d0",
			"#ee82ee",
			"#f5deb3",
			"#ffffff",
			"#f5f5f5",
			"#ffff00",
			"#9acd32"
		]
	}

#### Fail

	{
		error: 'Error message',
		status: 500
	}
