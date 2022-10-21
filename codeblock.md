## *Code Block*

This is my code block that I use for Calculus and Algebra equations. Great for when factoring is not an option. 

```python
from math import sqrt

check_input = True
while check_input:
    a, b, c = eval(input("Please enter the a, b, c coefficients of your quadratic equation: "))
    try: 
        float(a), float(b), float(c)
        check_input = False
    except ValueError:
        print("Please make sure the coefficients are real numbers and try again")
        check_input = True

disc = b*b-4*a*c

if disc >= 0:
    x1 = (-b+sqrt(disc))/(2*a)
    x2 = (-b-sqrt(disc))/(2*a)
    print("The roots of the equation are:", x1, x2)
else:
    print("The equation has no solutions")
```


### Site Navigation
<nav class="sitenavigation">
  <p><a href="README.md">Home</a></p>
  <p><a href="Gaming.md">Gaming</a></p>
  <p><a href="Music.md">Music</a></p>
  <p><a href="Snowboarding.md">Snowboarding</a></p>
</nav>