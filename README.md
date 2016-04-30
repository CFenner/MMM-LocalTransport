# MagicMirror-LocalTransport-Module

<p>
<a href="http://choosealicense.com/licenses/mit"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License"></a>
</p>

This module display the next local transport connection between an origin and destination.

![Sonos Module](https://github.com/CFenner/MagicMirror-LocalTransport-Module/blob/master/.github/preview.png)

## Installation

Go to your MagicMirror folder.

`cd MagicMirror`

Clone the repository.

`git clone https://github.com/CFenner/MagicMirror-LocalTransport-Module.git modules/localtransport`

## Configuration

Add module configuration to config.js.

```js
{
  module: 'localtransport',
  position: 'ANY_POSITION',
  config: {
    api_key: 'YOUR_API KEY',
    origin: 'YOUR_ORIGIN',
    destination: 'YOUR_DESTINATION'
  }
},
```

|Option|Description|
|---|---|
|`apiKey`|The API key, which can be obtained [here](https://developers.google.com/maps/documentation/directions/).<br><br>This value is **REQUIRED**|
|`origin`|The start location.<br><br>**Example:** `MannheimHBF`<br>This value is **REQUIRED**|
|`destination`|The target location.<br><br>**Example:** `Frankfurt HBF`<br>This value is **REQUIRED**|
|`maxConnections`|How many connections should be displayed?<br><br>**Default value:** `3`|
|`updateInterval`|How often does the content needs to be fetched? (Minutes)<br><br>**Default value:** `5`|
|`animationSpeed`|Speed of the update animation. (Seconds)<br><br>**Default value:** `1`<br><br>**Default value:** `3`|

## Special Thanks

Thanks to [SamLewis0602](https://github.com/SamLewis0602) and his module [MMM-Traffic by SamLewis0602](https://github.com/SamLewis0602/MMM-Traffic) on which this module is based on.
