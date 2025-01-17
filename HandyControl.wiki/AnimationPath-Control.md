AnimationPath Control enable you to use a geometric path to generate output values.

# Usage
First add HandyControl refrence
```
 xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:AnimationPath Duration="0:0:4" Data="M40.493382,19.001303 C36.637875,19.06448 33.938568,21.421986 33.948524,25.271919 L34.068279,71.56765 34.066906,71.598007 34.068745,71.747833 34.18895,118.21758 C34.202225,123.35083 39.026951,129.19344 44.965271,131.2674 50.903587,133.34137 55.706783,130.86133 55.693504,125.72808 L55.589508,85.524513 93.866371,85.524513 93.950943,118.21758 C93.964218,123.35083 98.788948,129.19344 104.72726,131.2674 110.66558,133.34137 115.46878,130.86133 115.4555,125.72808 L115.33575,79.432381 115.33712,79.401993 115.33528,79.252007 115.21507,32.782413 C115.2018,27.64917 110.37708,21.806566 104.43876,19.732603 98.500435,17.658638 93.697243,20.138674 93.710518,25.271919 L93.814514,65.475487 55.537647,65.475487 55.453079,32.782413 C55.439804,27.64917 50.615082,21.806566 44.676762,19.732603 43.192181,19.214111 41.778549,18.980244 40.493382,19.001303 z M9.999999,0 L140,0 C145.52284,0 150,4.4771523 150,9.999999 L150,140 C150,145.52284 145.52284,150 140,150 L9.999999,150 C4.4771523,150 0,145.52284 0,140 L0,9.999999 C0,4.4771523 4.4771523,0 9.999999,0 z"/>
```
| **Available Property** | **Description**                                             |
| ---------------------- | ----------------------------------------------------------- |
| Data                   | Geometry Image data                                         |
| PathLength             | Defines speed of drawing the shape                          |
| Duration               | Specifies the length of time it takes to complete the shape |
| Stroke                 | Specifies the brush color                                   |
| StrokeThickness        | Specifies thickness                                         |


***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/AnimationPath.gif)