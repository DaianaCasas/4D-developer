## Software Requirement 
•	Versión de 4D 17, Release3.
•	Objets
•	Macros
•	SVG component

##  Thermometer variable
In Formulary, create a new Image variable.
![image](https://github.com/DaianaCasas/4D-developer/assets/38088617/e419faea-58ca-44b6-af2e-551677d1fb97)

![image](https://github.com/DaianaCasas/4D-developer/assets/38088617/0f974992-ab39-4f41-9b6d-f95c74fa2f20)

Variable Name:
The variable Name and Object Name must be the same
![image](https://github.com/DaianaCasas/4D-developer/assets/38088617/08445970-1f2e-4a40-af7d-21dd78573f14)

Actions:
![image](https://github.com/DaianaCasas/4D-developer/assets/38088617/fe915387-ed08-4bc3-b43a-05d09c69981c)

Events:
![image](https://github.com/DaianaCasas/4D-developer/assets/38088617/c986931c-aa59-4fb6-b6a5-c0168c11746d)

Object Method:
Acces to Object Method of Image Variable and invoke thermometer function:
![createT](https://github.com/DaianaCasas/4D-developer/assets/38088617/b6749614-b890-4559-93b7-6cddb3356f19)

Other way to do it is selection in Macro icon and choose the Thermometer Function
![createT2](https://github.com/DaianaCasas/4D-developer/assets/38088617/cb1f5d60-a4ae-4e67-b2f3-3aabd8bca695)

Then a configuration window is opened:
![config1](https://github.com/DaianaCasas/4D-developer/assets/38088617/ea6d8c39-a6d1-48f0-b168-00ce4865fd9f)

![config2](https://github.com/DaianaCasas/4D-developer/assets/38088617/9425d637-8d24-4a6c-b424-d6f98774a1da)

![config3](https://github.com/DaianaCasas/4D-developer/assets/38088617/5b2531a1-c5ef-4d21-9e83-f40cd221dbd5)

![config4](https://github.com/DaianaCasas/4D-developer/assets/38088617/17ef73dd-e787-4092-86d8-6b736ae9df9c)

### Upate value thermometer

The functions uses a different image object name. Its generated a new name: *<object_name>_obj*
Example:

![ex](https://github.com/DaianaCasas/4D-developer/assets/38088617/9e62a67d-9044-4c5c-8e46-74261e48afd4)/

Case of 
	: (Form event=On Data Change)
		Termometro_UpdateValue (var1_obj; v1; "update")
End case
where v1 is a number variable.


Or
Case of 
	: (Form event=On Data Change)
		Termometro_UpdateValue (var1_obj; 50; "update")
End case 



## Add Thermometer Variable
Components:
Files:
+ termometro_base.txt
+ SVGMacros.xml

Project Methods:
 + termometro_create
 + termometro_updateValue

Proyect Form:
 + termometro_configurarGraduacion
