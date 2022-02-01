# GPS-location-

This project is an example of how the precise GPS locations in our cellular devices is calculated. For the simplicity of the project only the essential satellite data was used that is the latitude, longitude and the time of flight. To know the exact location we require four satellites the fourth one is to calculate the error from the location. 

The data from satellites is converted from spherical to cartesian coordinates. Further to solve for four unknown variables x,y,z and the time of flight Newton-Raphson method is used. In order to solve a system of non-linear equations it is necessary to represent the data in a Jacobian matrix. Multiple iterations of Newton-Raphsons methods must be implemented until the values get converged. The final step is to convert the cartesian coordinates back to spherical coordinates and cross verify the location using Google Maps.
