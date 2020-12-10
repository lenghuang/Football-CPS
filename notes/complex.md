# Complexities 

### Keeping track of things we may want to consider for the future:

- (Pass interference buffer:= * |=> buffer := 0)
- Curved OLine
- WR runs from line of scrimmage.. We can only throw in a range say 70-80 yards, to ensure we get as far as possible, but also, ensure that we can actually send the ball
- Generalize the starting position (issues --> if we are too close to 0, QB might run off the field, if we are too close to 300, there is less space to run forward)
- Instead of WR Open <=> pass, can calculate distance / time needed for a ball to travel for some velocity within the loop guard
- Another idea for WR Open : making it a function, and having it = prev def of Open & y >= 240
- Possibly introduce changing dy and vy, using controller first and then dy' and vy'

### What We Are Solving For:

##### Tradeoff between how far back LB starts and diffPass: 
- Given an arbitrary initial yLB, what is our minimum diffPass (and how does it change in relation to the QB's start)
- Given an arbitrary diffPass, what is the maximum initial LB (and how does it change in relation to the QB's start)
- Can we create/solve some multivariable equation that shows relation between diffPass, yLB, and yQB?


### Common Bugs:
- Lower bound by lower case `diff`
- Not expanding definitions 
- Forgetting that you hard coded `maxVel = vyD`

### Notes for Paper: 

- Have a paragraph for explaining Domain Constraints and why we have them in place
- Why we can have QB unhurt in domain constraint. Originally in Lab 2, we want to cover opposite case for ODE. But in diamond case, it's ok since it's \exists not \forall. If anything it's the responsibility of the angel / your agent to enforce the domain constraint.
