# SAP-Fiori-UI-Demo-Kit
This repository follow the UI Demo Kit Tutorial.

<strong> UI5 Conventions</strong>
	• View names are capitalized
	• All views are stored in the view folder
	• Names of XML views always end with *.view.xml
	• The default XML namespace is sap.m
	• Other XML namespaces use the last part of the SAP namespace as alias (for example, mvc for sap.ui.core.mvc)
	• Controller names are capitalized
	• Controllers carry the same name as the related view (if there is a 1:1 relationship)
	• Event handlers are prefixed with on
	• Controller names always end with *.controller.js
	• Use sap.ui.define for controllers and all other JavaScript modules to define a global namespace. With the namespace, the object can be addressed throughout the application.
	• Use sap.ui.require for asynchronously loading dependencies but without declaring a namespace, for example code that just needs to be executed, but does not need to be called from other code.
Use the name of the artifact to load for naming the function parameters (without namespace).

<strong> Content </strong>
01 Ready...Steady...Go APP 
https://ui5.sap.com/#/topic/592f36fd077b45349a67dcb3efb46ab1

02 Walkthrough 
https://ui5.sap.com/#/topic/3da5f4be63264db99f2e5b04c5e853db
