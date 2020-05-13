---
layout: article
title: SOLIDWORKS macro finds intersection points between surface and curve
caption: Find Intersection Points Between Surface And Curve
description: Example demonstrates how to find the intersection points between selected plane or face with edge or sketch segment
lang: en
image: /solidworks-api/geometry/surface-curve-intersection.png/surface-curve-intersection.png.png
labels: [curve, evaluate, geometry, macro, points, solidworks api, spline, intersection, trimmed curve, vba]
---
{% include img.html src="surface-curve-intersection.png" height=300 alt="Intersection point between plane and sketch spline" align="center" %}

This example demonstrates how to find the intersection points between selected surface (plane or face) with curve (edge or sketch segment) using SOLIDWORKS API.

* Open Part document
* Select plane or any face as first selection object
* Select sketch segment (line, spline or arc) as second selection object
* Run the macro. As the result the 3D Sketch is created with points of intersection between selected objects

[ISurface::IntersectCurve2](http://help.solidworks.com/2018/english/api/sldworksapi/solidworks.interop.sldworks~solidworks.interop.sldworks.isurface~intersectcurve2.html) SOLIDWORKS API method is used to find the intersection points within the specified boundaries of curve and surface.

{% include_relative Macro.vba.codesnippet %}