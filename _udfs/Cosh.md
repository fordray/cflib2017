---
layout: udf
title:  Cosh
date:   2001-10-09T15:40:23.000Z
library: MathLib
argString: "x"
author: Joel Cox
authorEmail: jlcox@goodyear.com
version: 1
cfVersion: CF5
shortDescription: Returns the hyberbolic cosine of an angle.
tagBased: false
description: |
 Returns the hyberbolic cosine of an angle.  All angles are expressed in radians.

returnValue: Returns a numeric value.

example: |
 <CFSET x=Pi()/2>
   <CFOUTPUT>
   Given x=#x#<BR>
   The Cosh of #x# radians is: #Cosh(x)#
   </CFOUTPUT>

args:
 - name: x
   desc: Angle measured in radians.
   req: true


javaDoc: |
 /**
  * Returns the hyberbolic cosine of an angle.
  * 
  * @param x      Angle measured in radians. 
  * @return Returns a numeric value. 
  * @author Joel Cox (jlcox@goodyear.com) 
  * @version 1, October 9, 2001 
  */

code: |
 function Cosh(x)
 {
     Return((Exp(x) + Exp(-x)) / 2);
 }

oldId: 48
---

