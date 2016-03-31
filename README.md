### Bug report #14594

qgis 2.8.8-Wien

Symbology Maker line error when pen width less 0.265 mm (es. 0.25 mm)

1. bug.qgs (Qgis project)
2. TEST_BUG.SHP

I think the problem is related to:  mm to pixel conversion (0.264583333).

#### The triangle should be in the middle of the dashed line.

When pen width is **0.3** mm (OK) **BLACK**.
When pen width is less than 0.265 mm (es. **0.26** mm; create problems) **RED**.
![Example](https://github.com/laingit/qgis-alai-bug/blob/master/Example.PNG)

Here the **BLACK** LINE (ok)
![OK](https://github.com/laingit/qgis-alai-bug/blob/master/ok.PNG)

Here the **RED** LINE (ERROR)
![ERROR](https://github.com/laingit/qgis-alai-bug/blob/master/ERROR.PNG).

![qgis](https://github.com/laingit/qgis-alai-bug/blob/master/qgis.PNG).
