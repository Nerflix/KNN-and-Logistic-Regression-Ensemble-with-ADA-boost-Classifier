# KNN-and-Logistic-Regression-Ensemble-with-ADA-boost-Classifier
The dataset is synthetically generated based on this dataset. The data contains 136429 rows and 14 columns, 5 of which are binary features of failure areas and 1 binary feature indicating the presence of machine failure regarding the area.
Data description:

Column	Datatype	Desc
UDI	Int	Universal Device Identifier
Production Id	String	Unique Id, combination of Type variable followed by a number identifier
Type	String	Type of product/device (L/M/H)
Air Temperature	Float	Air temperature in Kelvin
Process Temperature	Float	Production process temperature in Kelvin
Rotational Speed	Int	Speed in RPM (Rotations Per Minute) calculated with the power of 2860W
Torque	Float	Torque in Nm (Newton Meter)
Tool Wear	Int	Time unit needed to wear down the product/tool
Machine Failure	Int	Machine Failure binary feature
TWF	Int	Tool Wear Failure binary feature
HDF	Int	Heat Dissipation Failure binary feature
PWF	Int	Power Failure binary feature
OSF	Int	Overstain Failure binary feature
RNF	Int	Random Failure binary feature
The binary features consist of a variable indicating whether there's a failure or not, followed by 5 variables indicating the area/cause of failure. 5 different area of variable is described as follow:

TWF (Tool Wear Failure) indicating industrial tool failure resulting in the need for equipment change and defective products.
HDF (Heat Dissipation Failure) indicating failure in heat dissipation during the production process.
PWF (Power Failure) indicating that the power supplied was not fit to the production process need resulting in a failure.
OSF (Overstain Failure) indicating failure involves product overstains which may be the result of high load and tension during production.
RNF (Random Failure) indicating that a random error causes the failure.
Types of products/devices are divided into 3 categories which are L (Low), M (Medium), and H (High). The distribution of the variable is as follows:

For each product type (H/M/L), tool wear increases by some time unit.
Rotational speed (RPM) calculated from a power of 2860 W, overlaid with a normally distributed noise.
There is no negative torque.
The data contains no null values but does contain zeros which may need further investigation.
0 has more value than 1 in every binary feature.
Every area of failure has different toleration related to the Type of the product, the higher the Type label the most tolerant it is to fault conditions.
