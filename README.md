# pajp
A tool for service pipe dimensioning within district heating applications.
Authors: Olle Penttinen and Pelle Penttinen
Date: 2021-09-22
Copyright: Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)

**********************************************************************
Disclaimer
**********************************************************************
The
**********************************************************************
Functionality
**********************************************************************
The inputs to the left are used to calculate a difference in enthalpy. 
The enthalpy difference is used to calculate a massflow in order to serve the substation with the stated power
Corresponding pressure drops, velocities and differential pressures are calculated and stored for the different pipe dimensions
Densities, viscosities and enthalpy are calculated based on IAPWS formulation
Friction factor is retrieved by solving the Colebrook-White equation iteratively
Warnings are raised if values are outside of known limits
Green color: Within limits
Yellow color: Pressure drop > 100 Pa/m, Flow velocity > 1 m/s, Flow velocity > 1.5 m/s
Red color: Flow velocity > 2 m/s in copper pipes, Flow velocity > 3 m/s in steel pipes, Differential pressure > 6 bar at customer, Differential pressure < 1 bar at customer
Additional comment regarding thermostatic bypass valves is raised at table footer if differential pressure > 2 bar at connection point

