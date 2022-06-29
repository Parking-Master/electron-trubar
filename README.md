# Electron TruBar (electron-trubar)
The fastest and easiest way to customize any electron app window through the main process.

## Installing it
```
npm install electron-trubar --save
```
## What it includes
`backgroundColor` - String | Color/Hex
<br>
`textColor` - String | Color/Hex
<br>
`seamColor` - String | Color/Hex
<br>
`seam` - Boolean | Seamless/Seam
<br>
`title` - String | Title/Text
<br>
`height` - Number | Integer/Float
<br>
`trafficLightX` - Number | Integer/Float
<br>
`trafficLightY` - Number | Integer/Float

## Definitions
`backgroundColor` - Controls the background color of the titlebar.
<br>
`textColor` - Controls the foreground color of the titlebar.
<br>
`seamColor` - Controls the seam color of the titlebar.
<br>
`seam` - Controls whether the seam is shown on the titlebar.
<br>
`title` - Controls the title for of the titlebar.
<br>
`height` - Controls the height of the titlebar.
<br>
`trafficLightX` - Controls the X Axis position of the traffic lights.
<br>
`trafficLightY` - Controls the Y Axis position of the traffic lights.

## Example
```
npm install electron-trubar --save
```

##### main.js
```
const { app, BrowserWindow } = require("electron");
const TruBar = require("electron-trubar");

app.on("ready", function() {
  const mainWindow = new BrowserWindow({ ... });
  TruBar(mainWindow, {
    backgroundColor: "#333",
    textColor: "#fff",
    seam: true,
    seamColor: "#eee",
    height: 20,
    trafficLightX: 6.5,
    trafficLightY: 6.5,
    title: "My app"
  });
});
```

### Output

<br>

#### White
![Example Titlebar (White)](https://raw.githubusercontent.com/Parking-Master/Parking-Master/main/img/white-bar.png)

#### Red
![Example Titlebar (Red)](https://raw.githubusercontent.com/Parking-Master/Parking-Master/main/img/red-bar.png)

#### Black
![Example Titlebar (Black)](https://raw.githubusercontent.com/Parking-Master/Parking-Master/main/img/black-bar.png)

## License
__MIT__