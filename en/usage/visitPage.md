# Visit page
## Fields
The displayed fields depend on the type of data. For each data type, if a field is fillable in APP, it is displayed in the page.

|  | Vecteur | Raster | Service | Ressource |
| ------ | :--------: |:------: | :-----------: | :------: |
| **Abstract** | - | - | - | - |
| Abstract | x | x | x | x |
| **History** | - | - | - | - |
| Creation date | x | x | x | x |
| Modification date | x | x | x | x |
| Validity start | x | x |  |  |
| Validity end | x | x |  |  |
| Collection context | x | x |  |  |
| Collection method | x | x |  |  |
| Update frequency | x | x |  |  |
|  Comments | x | x |  |  |
| **Attriutes** | - | - | - | - |
| Attributes table | x | x |  |  |

## Export (XML, print)
### Export in XML
### Export in pdf
It is possible to generate a pdf with the metadata file to print directly from OpenCatalog, by clicking on the printing button.

All the metadata currently available are printed.

## Use services
The conditions of use are explained in the Requirements.
### Visualisation of services
Visualisable data can be filtered using the action Visualisation in the filter Widget or directly in the URL link using the query criteria ```q=action:view```.

Visualisation links are generated for every service that satisfies the conditions of use.

![Visualisation services](/assets/usage/view.PNG)

For Feature Services, the semantic informations of a geometry are displayed in a pop-up on click.

![Displayed semantic informations](/assets/usage/semanticInfos.PNG)

### Export services
Extracting services is possible for every Feature Services satisfying the conditions of use.

![Extract](/assets/usage/extract.PNG)

Depending on the capabilities of the server, OpenCatalog generate a extraction form. The form offer every formats of interest available as well as all the layer's available coordinates systems.

![Extraction Form](/assets/usage/extractionModal.PNG)
