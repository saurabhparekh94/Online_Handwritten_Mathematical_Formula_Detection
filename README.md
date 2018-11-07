# Online_Handwritten_Mathematical_Formula_Detection
# Online_Mathematical_Formula_Detection

The Project aims at classifing, Segementing and Parsing Handwritten Mathematical Formula. 
Input - The input to our Project is Handwritten Trace Points in the inkml format.

Classification - Given a set of Trace points the Prohect classifies these trace points as digits(0-9),Alphambets(a-z), sumbols(+,-,=,*,/,=),punctions(COMMA,PERIOD) etc
Segmentation- From a given trace file the segmentation tries to identify individual trace points. 
Parsing- Parsig tries to Identify if the given symbol isto the right, top, bottom, subscript, superscript of the previous symbol.

=========================================================================================
REQUIREMENTS:

This system requires networkx library as dependency

pip install networkx 

=========================================================================================
To run the system execute following command 

python main.py path_to_inkml 'segment/perfect' [bonus]

"path_to_inkml" should be a directory containing all the inkml files.
The program does not recursively look for directory in directory.

Example : 
python main.py path_to_inkml segment

OR

python main.py path_to_inkml perfect

The bonus parser is only for perfectly segmented symbols
To run for bonus, execute following command

python main.py path_to_inkml perfect

"perfect" flag is for running parsing on perfectly segmented symbols
"segment" flag is for running parsing on strokes level input

=========================================================================================

Output files

At the end of execution, a folder will be generated named : input_directory_"output_lg"
This folder will contain all the .lg files for the inkml files given as input 

=========================================================================================

Source code

All the python files should be placed in same directory

=========================================================================================
