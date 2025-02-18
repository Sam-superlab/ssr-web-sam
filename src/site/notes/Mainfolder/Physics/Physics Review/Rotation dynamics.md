---
{"dg-publish":true,"permalink":"/Mainfolder/Physics/Physics Review/Rotation dynamics/"}
---

## Torque


## Moment of inertia
>[! note] **Basic Definition**: The moment of inertia ($I$) of a body is a measure of its resistance to a change in its rotational motion. 

***It's the rotational equivalent of the role played by mass in linear dynamics. Just like mass determines how much an object resists linear acceleration, the moment of inertia determines how much an object resists angular acceleration.***

2. **Calculation for Single Point Mass**: For a particle of mass \( $m$ \) rotating at a distance \( $r$ \) from an axis, the moment of inertia is \( $I = mr^2$ \). This formula applies to point masses, which are idealized particles that have mass but occupy no space.
3. **Extended to Complex Objects**: For an object consisting of multiple point masses, the moment of inertia is the sum of the moments of inertia of each point mass, calculated as \( $I = \sum mr^2$\). This summation represents adding the moments of inertia of each point mass (where \( $m_i$ \) is the mass of each point mass and \( $r_i$ \) is the distance of each mass from the axis of rotation). For example, for two bodies of equal mass, the moment of inertia would be \( $I = mR^2 + mR^2 = 2mR^2$ \) if each body is a distance \( $R$ \) from the axis.
4. **Dependence on Axis of Rotation**: The moment of inertia of an object significantly depends on the axis about which it is rotated. Different axes through the same object will generally yield different moments of inertia.
5. **Units of Measurement**: The moment of inertia is measured in kilogram meters squared (kg m²).

## Energy in Rotation
1. **Rotational Kinetic Energy**: The rotational kinetic energy is given by $$E_{K, \text{rot}} = \frac{1}{2}I\omega^2$$, where \( I \) is the moment of inertia and \( \omega \) is the angular speed.

2. **Translational Kinetic Energy**: The translational kinetic energy is given by $$E_{K, \text{trans}} = \frac{1}{2}mv^2$$, where \( m \) is the mass of the object and \( v \) is its translational (linear) speed.

3. **Total Mechanical Energy**: The total mechanical energy of an object that is both rotating and moving linearly is the sum of its rotational and translational kinetic energies, expressed as:
   $$E_T = \frac{1}{2}I\omega^2 + \frac{1}{2}mv^2$$
   If gravitational potential energy is also involved, the equation includes this term as well:
   $$E_T = \frac{1}{2}I\omega^2 + \frac{1}{2}mv^2 + Mgh$$

4. **Example Scenario**: In a system like a flywheel, where gravitational potential energy is converted into kinetic energies, the energy conservation equation can be written as:
   $$mgh = \frac{1}{2}mv^2 + \frac{1}{2}I\omega^2 + W$$
   Here, \( W \) represents the work done against friction.
