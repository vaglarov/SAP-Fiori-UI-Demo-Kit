# SAP-Fiori-UI-Demo-Kit
This repository follow the UI Demo Kit Tutorial.

<strong> UI5 Conventions</strong>
<p><ol>
	<li> View names are capitalized</li>
	<li> All views are stored in the view folder</li>
	<li> Names of XML views always end with *.view.xml</li>
	<li> The default XML namespace is sap.m</li>
	<li> Other XML namespaces use the last part of the SAP namespace as alias (for example, mvc for sap.ui.core.mvc)</li>
	<li> Controller names are capitalized</li>
	<li> Controllers carry the same name as the related view (if there is a 1:1 relationship)</li>
	<li> Event handlers are prefixed with on</li>
	<li> Controller names always end with *.controller.js</li>
	<li> Use sap.ui.define for controllers and all other JavaScript modules to define a global namespace. With the namespace, the object can be addressed throughout the application.</li>
	<li> Use sap.ui.require for asynchronously loading dependencies but without declaring a namespace, for example code that just needs to be executed, but does not need to be called from other code.</li>
	<li>Use the name of the artifact to load for naming the function parameters (without namespace).</li>
	<li>The resource model for internationalization is called the i18n model.</li>
	<li>The default filename is i18n.properties.</li>
	<li>Resource bundle keys are written in (lower) camelCase.</li>
	<li>Resource bundle values can contain parameters like {0}, {1}, {2}, …</li>
	<li>Never concatenate strings that are translated, always use placeholders.</li>
	<li>Use Unicode escape sequences for special characters.</li>
	<li>Do not specify colors in custom CSS but use the standard theme-dependent classes instead.</li>
</ol>
</p>
<strong> Content </strong>
<p>
01 Ready...Steady...Go APP 
https://ui5.sap.com/#/topic/592f36fd077b45349a67dcb3efb46ab1

02 Walkthrough 
https://ui5.sap.com/#/topic/3da5f4be63264db99f2e5b04c5e853db
</p>

</p>
<strong> Helpful terminologies </strong>
	<p><ol>
	<li> <strong> index.html </strong>
		<p>  
		An HTML document consists basically of two sections: head and body. The head part will be used by the browser to process the document.
		Using meta tags, we can influence the behavior of the browser. In this case, we tell the browser to use UTF-8 as the document character set.
		We also give our app a title that will be displayed in the browser. Our hard-coded title can be overruled by the app, for example to show a title in the language of the user. The body part describes the layout of the 		page. In our case, we simply display "Hello World" by using a div tag.
		</p>
	</ol>
    </p>
<p>
