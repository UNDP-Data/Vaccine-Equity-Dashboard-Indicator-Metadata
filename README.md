# Vaccine Equity Dashboard Indicator Metadata

Metadata for the indicators in the vaccine quity dashboard

Vaccine Equity Dashboard on DFP: https://data.undp.org/vaccine-equity

## Data Structure of an object

Key | DataType | Description
--- | --- | --- 
Theme | `string` | Available Values: "", "Affordability", "Accessibility"
Indicator | `string` | Short description of the indicator
IndicatorDescription | `string` | Long description of the indicator
DataKey | `string` | Name or Key by which the indicator data is stored in the data sheet csv
DataSourceName | `string` | Name of the source from which this indicator data is fetched
DataSourceLink | `string` | Weblink to the source
LabelSuffix | `string` | Suffix to the data for the indicator when shown on mouseover. For ex if the `LabelSuffix` is `%` and the data for the indicator is `80` then on mouse over the data would be shown as `80 %`
LabelPrefix | `string` | Prefix to the data for the indicator when shown on mouseover. For ex if the `LabelPrefix` is `US$` and the data for the indicator is `80` then on mouse over the data would be shown as `US$ 80`
LabelFormat | `string` | Currently not in used, but needed. Therefor the valuer currently is always _""_
BinningRange5 | `[number, number, number, number]` | An array of 4 numbers defining the domain for threshold scale in bivariate choropleth map. _If the indicator has categorical data the value of this need to be `[]`_
BinningRangeLarge | `number[]` | An array of  numbers defining the domain for threshold scale in single variate choropleth map. The length of array can vary from 4 to 10. _If the indicator has categorical data the value of this need to be `[]`_
Categories | `number[] or string[]` | An array of  numbers or string defining the categories if the the indicator has categorical data. The length of array can be 5, 7 or 10. _If the indicator is not categorical in nature value of this need to be `[]`_
CategorizeByRanking | `boolean` | Currently not in use
IsCategorical | `boolean` | Define if the indicator is categorical in nature or not
IsDivergent | `boolean` | Define if the indicator data is divergent in nature or not. This defines the colors that are used for choropleth map. If `true` a divergentcolor scheme is used otherwise a linear color schame is used
ScatterPlot | `boolean` | Define if the indicator can be visualized in scatterplot (generally categorical data are not visualized as scatter plot)
Map | `boolean` | Define if the indicator can be visualized as color in choropleth map
BarGraph | `boolean` | Define if the indicator can be visualized as bars in bar graph (generally categorical data are not visualized as scatter plot)
Sizing | `boolean` | Define if the indicator can be visualized as the size or bubble in scatterplot or as an overlay on the map (generally categorical data and data which can have negative values are not visualized as area)
Color | `boolean` | Define if the indicator can be visualized as color of bubbles in scatterplot and bar chart (only categorical data are visualized as colors in scatter plot and bar chart)
