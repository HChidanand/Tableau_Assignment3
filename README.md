 
"# Tableau_Assignment3" 
Import Data Source File as text file

# Open Worksheet1
Drag worldwide gross measure to Rows and select measure as SUM.
Drag Genre Dimension to column.
Marks Genre into colour and worldwide gross measure to LEBEL marks
Rename worksheet1 as " Worldwide Gross Profit By Genre"

# Open Worksheet2
Drag worldwide gross measure to Rows
Drag Year Dimensions to Column
Marks Genre dimensions into column and select mark dropdown as area instead of Automatic
Rename worksheet2 as " Worldwide Gross Profit 2006 - 2012 "

# Open Worksheet3
Drag Lead Studio To Column
Drag Profitability to Rows
Go to Show Me Pane and select packaged bubble graph
Drag Lead Studio to colour marks & lable Marks
Apply filter to profitability
Rename Worksheet3 as " Lead Studio Profitability "

# Open Worksheet4
Drag film dimensions to rows
Drag Rotten Tomatoes % to column
Apply Filter to Genre & select show filter
Drag Rotten tomatoes % to colour marks and edit colour as Orange Light
# Now here I want assign Tomatometer Retings Symbols w.r.t films as per standard
# Here I have create Calculated field for rotten tomatoes% named as Tomatomere Ratings & Calculation Field Program as below
---IF [Rotten Tomatoes %] <60 THEN "Rotten"
   ELSEIF [Rotten Tomatoes %]>60 AND [Rotten Tomatoes %]<75 THEN "Fresh"
   ELSE "Certified_Fresh"
   END
---
Created Tomatometer Ratings Dimension inside the Dimesion part
Ctrl+Drag rotten tomatoes% from column to right and created one more graphs inside canvas
Go to marks and select 2nd measure and click on shapes
Drag Tomatometer rating to shapes inside 2nd graphs
Assign Tomatometer Rating Symbols to selected data item w.r.t images of symbols by selecting shape pallet from dropdown as a Tomatometer Symbols & rotten Tomatoes into lables.
# Here Tomatometer Symbol Pallet loaded by below path i.e Documents/My Tableau Repository/Shapes/Tomatometer Symbol/Images
Incraese Size of shapes as best fit
Now go to top of workbook and select 2nd measure into columns and select as dual axis from dropdown
Go to 1st measure inside marks and select BAR drom in dropdown list instead of automatic.
Update axis name as " Rotten tomatoes[%] by Tomatometer Ratings"
Rename Worksheet Title as " Genrewise List of Film with Tomatometer Rating "

# Open Dashboard1
Drag 2 Horizontal and 1 vertical object into dashboard canvas
Inside Horizontal1 drag 3 Vertical object & Inside Horizontal2 drag 2 Vertical Object
Drag " Worldwide Gross Profit By Genre" inside Vertical1 object
Drag " Worldwide Gross Profit 2006 - 2012 " inside vertical2 object
Drag " Lead Studio Profitability " inside vertical3 object and drag all filter and legends inside vertical1
Drag " Genrewise List of Film with Tomatometer Rating " inside horizontal2