---
title: HackerRank-Find_the_Torsional_Angle
date: 2021-02-09 23:47:00
tags: python, dot product formula, vector cross product formula 
---
# HW - Find the Torsional Angle

### Given code:
```
import math

class Points(object):
    def __init__(self, x, y, z):

    def __sub__(self, no):

    def dot(self, no):

    def cross(self, no):
        
    def absolute(self):
        return pow((self.x ** 2 + self.y ** 2 + self.z ** 2), 0.5)



if __name__ == '__main__':
    points = list()
    for i in range(4):
        a = list(map(float, input().split()))
        points.append(a)

    a, b, c, d = Points(*points[0]), Points(*points[1]), Points(*points[2]), Points(*points[3])
    x = (b - a).cross(c - b)
    y = (c - b).cross(d - c)
    angle = math.acos(x.dot(y) / (x.absolute() * y.absolute()))

    print("%.2f" % math.degrees(angle))
```
<br>
<hr>

### Start coding on paper
<br>
<img src="" alt="손코딩1">

<img src="" alt="손코딩2">

---

### Coding on Jupyter
<br>
<img src="" alt="jupyter에서 한 코딩 캡쳐본">