# Collecting data on employment in the labor market - data werehouse project

## Project contains
1. **Designed data warehouses** for employment data on the labor market.
2. **Implementation of ETL processes** loading information from the [csv file]() to the data warehouse. 
3. **Implementation of analytical business reports** used to visualize statements of data from the data warehouse.

### Project video presentation
[![YouTube video](http://img.youtube.com/vi/KEnFCFeLJWI/0.jpg)](http://www.youtube.com/watch?feature=player_embedded&v=KEnFCFeLJWI)

## Description of the steps
1. The data warehouse should collect data on the number of people working with regard to: industry (branża), location (lokalizacja), gender (płeć) and age range (przedział wieku).
According to the [csv file](), identify which of the of the listed attributes are **dimensions** and which represent a **measure**.
Then a [**star-shape diagram**]() should be developed with the necessary **dimension tables** and
**fact table**. All designed tables should be on the **graphical diagram**. 
2. Using the _Pentaho Data Integration_ tool, you should implement [ETL processes]() that
will allow you to load data from the provided [csv file]() into the data warehouse tables with
[star-shape diagram](). Note the following difficulties:
    - The data are contaminated and should be ETL corrected, e.g. size
    letters in industry names (eg "Edukacja", "EdukacjA"), short or full gender name
    (eg "K", "kobiety"), excess spaces (eg "Transport, gospodarka 
    magazynowa___i łączność")
    - The age dimension is written in columns instead of rows; it is necessary
    "rotating" the columns with age brackets to a vertical layout
    - the [csv file]() uses national character encoding compatible with Windows1250
3. Using Pentaho Report Designer you need to implement three analytical business reports. They must in these reports
the following elements may occur:
    - presentation of data in [**tabular form**]()
    - presentation of data in the form of a [**graphical chart**]()
    - data presentation in the form of a [**pivot table**]() (matrix layout)
    - report **calling parameter**, entered by the user
    - a **graphic element**, e.g. a logo
