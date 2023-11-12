# ExcelInterface_GLYCIM
An Excel based interface for the soybean model GLYCIM
An excel based interface to create the input files needed for the crop models 

The input data are stored in an excel spreadsheet. 

A special Excel file contains VBA code to pull data from the spreadsheet and create the folder structure and input files needed to run maizsim. The VBA program generates grid1.bat files in each folder that will create the grid and soil files when run. Only the weather files are not created. 

the Models.zip file has the executables 

Working examples include data for a soybean simulation from a FACE experiment in Iowa


To run the model, use the root folder set in the excel interface.
let's say the root is d:/IllFace and under this are the data folders,IllFACE_01 and IllFACE_02
then the executables would go into the IllFace folder and you would run the model as
d:/IllFace > 2dmaizsim ./IllFace_01/IllFace_01.dat

if you use the folder structure in this repository

Y:\ExcelInterface_Glycim
you would run the model as:
2dGlycim ./"Example input/IllFace_01/IllFace_01.dat"
Your files would be set up this way in the interface:
Input excel file:	Y:\ExcelInterface\Example input\SoybeanInputs.xlsx
Root Path:	Y:\ExcelInterface\Example input
MaizsimPath	Y:\ExcelInterface
CreateSoils	Y:\ExcelInterface\CreateSoilFIles
ExcelInterface	Y:\ExcelInterface\ExcelInterface
Weather CSV File Folder	Y:\ExcelInterface\Example input\

