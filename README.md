# pajp
A tool for service pipe dimensioning within district heating applications.

Authors: Olle Penttinen and Pelle Penttinen

Date: 2021-09-22

**********************************************************************
Disclaimer
**********************************************************************
None of the authors is responsible for your use of the information contained in or linked from these web pages and any implications that may lead to. 
The authors assumes no responsibility or liability for any errors or omissions in the content of this site. 
The information contained in this site is provided on an "as is" basis with no guarantees of completeness, accuracy, usefulness and without any warranties of any kind whatsoever, expressed or implied.
**********************************************************************
Functionality
**********************************************************************
The inputs to the left are used to calculate a difference in enthalpy. Preset values are entered to trigger three types of warning badges among the results. The enthalpy difference is used to calculate a massflow in order to serve the substation with the stated power. Corresponding pressure drops, velocities and differential pressures are calculated and stored for the different pipe dimensions.

Densities, viscosities and enthalpies are calculated based on IAPWS formulation. Friction factor is retrieved by solving the Colebrook-White equation iteratively. Warnings are raised if values are outside of known limits:

Green color: Within limits

Yellow color: Pressure drop > 100 Pa/m, Flow velocity > 1 m/s, Flow velocity > 1.5 m/s

Red color: Flow velocity > 2 m/s in copper pipes, Flow velocity > 3 m/s in steel pipes, Differential pressure > 6 bar at customer, Differential pressure < 1 bar at customer

An additional comment regarding thermostatic bypass valves is raised at table footer if differential pressure > 2 bar at connection point

## License
[Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/)
