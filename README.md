# integ
Solve counter integrated functions by finite combination.

# Description
If there's a integrate equation that describes each other by geometry,
the original integrated function is also effected by another geometry on them.

Stub.

This is the analogy to get last line of life game with floating point, multiple dimension.

# Detail
f(x,y,z) := Integrate Integrate Integrate dx dy dz f(x,y,z) \* I(x,y,z)  
I(x,y,z) := Integrate Integrate Integrate dx dy dz g(f) \* J(x,y,z)

We define with tensor way, but if it's in 2d it's the form:  
f = Integ(x) I_x f I_y Integ(y)  
I = Integ(x) J_x g(f) J_y Integ(y)

f = Integ(x) (Integ(x) J_x g(f) J_y Integ(y))\_x f (Integ(x) J_x g(f) J_y Integ(y))\_y Integ(y)

Given g as tangent form in randtools, we want: I, J, f.

f = A J_x arctan(tan(B_x f B_y)) J_y C f C^t J_x arctan(tan(B_x f B_y)) J_y A^t

Collecting another half pair to make them symmetric, it's equivalent to:

\[\[I f-I\],\[(f-I)^t I\]\] = \[\[J_x^2J_y^2g^2(f)f ...\], ...\]
