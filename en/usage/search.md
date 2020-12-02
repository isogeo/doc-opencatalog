# Search
OpenCatalog has a search engine as well as a filter width allowing quick access to the desired metadata page, making it possible to find one or more specific data.

## Filters
There are two tools to filter datasets :
* A filter widget
* A search bar

### Filter widget
It is possible to filter by the following criteria :
* An input text contained in : title, name, abstract, layer name or attribute name in attribute table,
* the owner if data from multiple work groups are shared,
* one or more Isogeo keywords,
* data type,
* data format,
* coordinates system,
* one or more Inspire themes,
* one or more action,
* one or more license,
* one or more contact.

Once a filter is selected, the result number as well as other possible filter values are updated. If a new filter is selected and there is only one value in another filter, this filter is automatically selected.

![FilterWidget](/assets/usage/filterWidget.PNG)

#### Other
The filters are applied following a 'strict and' rule, meaning all criteria must be met in order for the data to be displayed.

### Search Bar

A search bar is also available
![Search bar](/assets/usage/researchBar.png)

#### How to use : Autocomplete

To use the autocomplete search bar, start by adding the tags followed by the input text.

#### How to use : Tag nomenclature
It is also possible to use directly the Isogeo tag nomenclature to query data.

| Field | Query nomenclature |
|:------:|:----------------------------------:|
| Owner | `owner:` followed by the owner id |
| Keywords | `keyword:isogeo` followed the keyword tag |
| Type | `type:` followed by the type tag |
| Format | `format:` followed by the format tag |
| Coordinate system | `coordinate-system:` followed by the system tag |
| Inspire themes | `keyword:inspire-theme:` followed by the correct tag |
| Action | `action:` followed by the action tag |
| License | `license:` followed by the license id |
| Contact | `contact:` or  `contact:group:` depdending on contact type, followed by the contact id |

For instance, querying the string `coordinate-system:2154 action:download` renders the same result as selecting Lambert-93 coordinate system et Download action.

This nomenclature is used in URL when a query is made.

#### Other
* As well as the filter widget, the data are displayed only if all criteria are met.
* Warning : Unlike the filter widget, the "Undefined" value is possible for every field even if no data meet this specific criterion as long as no other value is selected for this field.

## Sort
Data can be sorted using two criteria :
* sort order : descendant and ascendant
* sort object : alphabetic order, relevence, metadata last update and data last update
