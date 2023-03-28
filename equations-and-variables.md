# Fluid-Mechanics-Equations-and-Units

## Unit Symbol Definitions  
$m$: meters  
$cm$: centimeters  
$g$: grams  
$kg$: kilograms  
$s$: seconds  
$N$: Newtons  

## Variables with Units  
length(l), height (h), or width (w) [=] $m$  
diameter (D) or radius (r) [=] $m$  
area (A) [=] ${m^2}$  
volume (V) [=] $cm^3$ or ${m^3}$  
mass (m) [=] $g$ or $kg$  
time (t) [=] $s$  
velocity (v or u) [=] $m/s$  
gravity (g) [=] $m/s^2$  
weight(W) [=] $kg {\cdot m/ s^2}$  
force (F) [=] $kg {\cdot m/ s^2}$  
density ($\rho$) [=] $g/cm^3$ or $kg/m^3$  
pressure (P) [=] $kg/{m \cdot s^2}$  
viscosity ($\mu$) [=] $kg/{m \cdot s}$  
specific weight ($\gamma$) [=] $N/m^3$  
specific gravity (SG) [=] unitless ($\gamma_x$/ $\gamma_{H_{2}O}$) where $x$ is the specified liquid or sample  
volumetric flow rate (Q) [=] ${m^3/s}$  
torque (T) = r x F [=]  $kg {\cdot m^2/ s^2}$  
stress ($\tau$) [=] $kg/{m \cdot s^2}$  
angular velocity ($\omega$) [=] $1/s$ (radians per second)  
theta ($\theta$) [=] radians  

## Equations

### Fluid Statics
$P = {\rho} gh = {\gamma} h$  
$P = F/A$  
$W = {\rho} gV$ (also Buoyancy)  

----------------------------------------

### Fluid Kinematics (micro/differential)

Conservation of Mass: $\frac{\partial \rho}{\partial t} +\underline{\nabla} \cdot (\rho \underline{v}) = 0$  

- if $\rho$ is constant, $\underline{\nabla} \cdot \underline{v} = 0$  

Conservation of Momentum:

General:  

$\rho \frac{D\underline{v}}{Dt}  = \rho \underline{g} - \underline{\nabla} P + \underline{\nabla} \cdot \underline{\underline{\tau}}$  

$\rho \frac{\partial \underline{v}}{\partial t} + \rho \underline{v} \cdot \underline{\nabla} \underline{v} = \rho \underline{g} - \underline{\nabla} P + \underline{\nabla} \cdot \underline{\underline{\tau}}$  

Navier-Stokes:  

$\rho \frac{\partial \underline{v}}{\partial t} + \rho \underline{v} \cdot \underline{\nabla} \underline{v} = \rho \underline{g} - \underline{\nabla} P + \mu \nabla^2 \cdot \underline{v}$

----------------------------------------------

### Fluid Kinematics (macro)

Conservation of Mass:  

$\frac{dm}{dt} = \rho \int_{CS_{entrance}} \ v \ dA - \rho \int_{CS_{exit}} \ v \ dA$  

$\rho \frac{dV}{dt} = \rho \int_{CS_{entrance}} \ v \ dA - \rho \int_{CS_{exit}} \ v \ dA$  

$\frac{\partial}{\partial t} \int_{CV} \ \rho \ dV = - \int_{CS} \rho \underline{v} \cdot \underline{n} \ dA$   (same as)   $ \rho Q_1 = \rho Q_2$  

Conservation of Momentum:

$\frac{\partial}{\partial t} \int_{CV} \rho \underline{v} \ dV \ + \int_{CS} \rho \underline{v} (\underline{v} \cdot \underline{n}) \ dA = \sum \underline{F}$  

Conservation of Energy (Bernoulli's Equation):

$\dot{Q} + \dot{W} = \int e \rho \underline{v} \cdot \underline{n} \ dA$

With the following assumptions
- steady flow
- $\rho$ is constant
- neglect friction, shear stress and viscous stress
- one entrance and one exit with constant properties
- constant volume  

We get: $\frac{P_1}{\rho g} + z_1 + \frac{v_1^2}{2g} = \frac{P_2}{\rho g} + z_2 + \frac{v_2^2}{2g}$  where "1" denotes the entrance and "2" denotes the exit

Modified Bernoulli's Equation (including fritional stresses, pumps, fans, and turbines):  

$\frac{\dot{W}}{\rho g Q} = (\frac{1}{2} \frac{<v>^2}{g}+z+\frac{P}{\rho g})_2 + (\frac{1}{2} \frac{<v>^2}{g}+z+\frac{P}{\rho g})_1$  

$\frac{\dot{W}}{\rho g Q} = f \frac{<v>^2}{2g} \frac{L}{D}$  

where $f$ is the friction factor that depends on the Reynolds Number and Roughness ($\frac{\epsilon}{D}$)  

-------------------------------------
  
### Flow over surfaces

Reynolds Number (Re): $\frac{\rho u L}{\mu}$  

Drag Force: $C_D \frac{1}{2} \rho u^2 A$ where $C_D$ depends on shape, oreientation, and Re  

Lift Force: $C_L \frac{1}{2} \rho u^2 A$  

-------------------------------------
  
### Boundary Layer

Boundary Layer Thickness: $\delta = 1.721x / \sqrt{Re_x}$  

where $Re_x = \frac{\rho u x}{\mu}$  

Drag Force: $C_{D_L} \frac{1}{2} \rho u^2 A$ where $C_{D_L}$ is $C_D$ for a given length of wall L (average $C_D$ over whole L)


