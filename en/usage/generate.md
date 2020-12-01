# Generate
## Generate a consultation catalog with openCatalog
To create an instance of OpenCatalog, do the following :

1. In the `Aministration` > `Inventory` > `Shares`, click on `New`
2. Click on the gearwheel
3. Select application `OpenCatalog`
4. Sekect the catalog(s) to publish
5. Name the Shares
6. `Create`

The consultation URL is displated.

![Manage the catalogs](/assets/usage/generateOC.PNG)

## Chose color
It is possible to integrate OpenCatalog directly in a webSite. If you want to fit the OpenCatalog colors to your organism's graphical charter, it is possible to chose one main color.

To change this main color :
1. In the `Administration` > `Isogeo` > `Settings`, change the color.

To go back to the original color, click on the large cross in the color picker.

![Change the color](/assets/usage/colorPicker.PNG)

## Integrating the OpenCatalog in a website (iframe)
OpenCatalog is developed via the Isogeo API. It was designed to be easily integrated in existing websites (intranet, extranet, mapping portal, OpenData portal, spatial data infrastructure, etc.) via an [iFrame HTML tag](https://www.w3schools.com/tags/tag_iframe.asp).

Multiples modes were implemented in the OpenCatalog.

### Removing the header
It is possible to remove the header.

#### How to use
To use this mode, simply add ``?no-header`` to the URL.

For instance, to integrate the demonstration OpenCatalog, use the following code :
```
<iframe src="https://open.isogeo.com/s/8d491301f61249139918e3710cd39eb7/wak8OBU2hQX6F6rtIe3fWiRCvzFH0?no-header" width=100% height="800"></iframe>
```

### Integrating a single page
If you want to integrate a single record, for example in a pop-up window, use the ``?lock`` mode.

There are the following differences between this mode and an OpenCatalog with no mode used :
* The header is removed
* Navigation from one page to another is not possible : If the "locked" page is a metadata record, it is impossible to go back to the records list ou go to an associated record page. If the "locked" page is the records list, it is impossible to click on a specific record.

#### How to use
To use it, simply add ``?lock`` at the end of the web address.

For instance :
```
<iframe src="https://open.isogeo.com/s/8d491301f61249139918e3710cd39eb7/wak8OBU2hQX6F6rtIe3fWiRCvzFH0?lock" height="400"></iframe></a>
```

### Remove services and resources
There are four record types :
* Raster dataset
* Vector dataset
* Resource
* Service

If you want to only show datasets, use mode ``?dataset-only``.

#### How to use
To use it, simply add ``?dataset-only`` at the end of the web address.

For instance :
```
<iframe src="https://open.isogeo.com/s/8d491301f61249139918e3710cd39eb7/wak8OBU2hQX6F6rtIe3fWiRCvzFH0" height="400"></iframe></a>
```

### Disabling proxy
To fetch informations about the services despite Criss-Origin issues, OpenCatalog uses a proxy. However, this prevent the OpenCatalog to query "local" services (any services only available locally : local computer or intern server). To access those services from the site, the proxy must be disabled.

#### How to use
To use this mode, just add ``?no-proxy`` at the end of the link. For instance, to integrate the demonstration catalog.
```
<iframe src="https://open.isogeo.com/s/8d491301f61249139918e3710cd39eb7/wak8OBU2hQX6F6rtIe3fWiRCvzFH0?no-proxy" width=100% height="400"></iframe>
```
#### Enable Cross Origin
Disabling the proxy might cause CORS issues. Therefor the server associated must recognize the OpenCatalog as allowed to access the server.
```
Access-Control-Allow-Origin: https://open.isogeo.com
```
Informations to specific server can be found [here](https://en.wikipedia.org/wiki/Cross-origin_resource_sharing).
