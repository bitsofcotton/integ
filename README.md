# integ
Solve counter integrated functions by finite combination.

# Description
If there's a integrate equation that describes each other by geometry,
the original integrated function is also effected by another geometry on them.

Stub.

This is the analogy to get last line of life game with floating point, multiple dimension.

# Detail
f(x,y,z) := Integrate Integrate Integrate dx dy dz f(x,y,z) \* I(x,y,z)  
I(x,y,z) := Integrate Integrate Integrate dx dy dz g(f) J(x,y,z)

We define with tensor way, but if it's in 2d it's the form:  
f = Integ(x) I_x f I_y Integ(y)  
I = Integ(x) J_x g(f) J_y Integ(y)

f = Integ(x) (Integ(x) J_x g(f) J_y Integ(y))_x f (Integ(x) J_x g(f) J_y Integ(y))_y Integ(y)

Given g as tangent form in randtools, we want: I, J, f.

