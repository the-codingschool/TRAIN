**Dataset description:**

**Source:** This dataset was created from a subset of data from [SimpleMaps.com](https://simplemaps.com/data/us-counties)

<br />

**Files:**
- `us_counties.csv` - Cleaned dataset.
- `visualizing_county_maps.ipynb` - Includes examples/demos of what this dataset would be used to teach.
- `topo_map.png` - (image) Topographical map of the US that is used in the notebook.

<br />

**Note:** Some counties may appear to be duplicates with similar names, this is NOT a mistake. Double check the associated state as many states have counties with the same name. In other instances, several larger cities started out being part of a county of the same name but eventually grew too big and broke off to become its own county (ex: Baltimore). In these cases, the city that broke off is labelled "Baltimore City" while the original county is still just "Baltimore".

**Attribute Information:**

|     |     |     |
| --: | --- | --- |
|  1. | county | Name of the county |
|  2. | state | State abbreviation *(ex: NY, CA, TX)* |
|  3. | population | An estimate of the county's population (as of Feb 2024) |
|  4. | latitude | Latitude of the county (approx center point) |
|  5. | longitude | Longitude of the county (approx center point) |

<br />

Good for EDA / data visualizations, specifically to create maps. Not intended for ML applications.

<br />

```
import pandas as pd
url = "https://raw.githubusercontent.com/the-codingschool/TRAIN/main/us_counties/us_counties.csv"
df = pd.read_csv(url)
```
