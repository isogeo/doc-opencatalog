# Search
## Filters
There are two tools to filter datasets :
* A filter widget
* A search bar

### Filter widget

The filters are applied following a 'strict and' rule, meaning all criteria must be met in order for the data to be displayed.

![FilterWidget](/assets/usage/filterWidget.PNG)

### Search Bar

A search bar is also available
![Search bar](/assets/usage/researchBar.PNG)

#### How to use : Autocomplete

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

#### Characteristics
As well as the filter widget, the data are displayed only if all criteria are met.

## Sort
Data can be sorted using two criteria :
* sort order : descendant and ascendant
* sort object : alphabetic order, relevence, metadata last update and data last update
