# SAP-Fiori-UI-Demo-Kit
This repository follow the UI Demo Kit Tutorial.
https://ui5.sap.com/#/topic/8b49fc198bf04b2d9800fc37fecbb218

<strong> UI5 Conventions</strong>
<p><ol>
	<strong> XML Views</strong>
	<li>View names are capitalized</li>
	<li>All views are stored in the view folder</li>
	<li>Names of XML views always end with *.view.xml</li>
	<li>The default XML namespace is sap.m</li>
	<li>Other XML namespaces use the last part of the SAP namespace as alias (for example, mvc for sap.ui.core.mvc)</li>
	<strong> Controllers</strong>
	<li>Controller names are capitalized</li>
	<li>Controllers carry the same name as the related view (if there is a 1:1 relationship)</li>
	<li>Event handlers are prefixed with on</li>
	<li>Controller names always end with *.controller.js</li>
	<strong> Modules</strong>
	<li>Use sap.ui.define for controllers and all other JavaScript modules to define a global namespace. With the namespace, the object can be addressed throughout the application.</li>
	<li>Use sap.ui.require for asynchronously loading dependencies but without declaring a namespace, for example code that just needs to be executed, but does not need to be called from other code.</li>
	<li>Use the name of the artifact to load for naming the function parameters (without namespace).</li>
	<strong> Translatable Texts</strong>
	<li>The resource model for internationalization is called the i18n model.</li>
	<li>The default filename is i18n.properties.</li>
	<li>Resource bundle keys are written in (lower) camelCase.</li>
	<li>Resource bundle values can contain parameters like {0}, {1}, {2}, …</li>
	<li>Never concatenate strings that are translated, always use placeholders.</li>
	<li>Use Unicode escape sequences for special characters.</li>
	<strong> Component Configuration</strong>
	<li>The component is named Component.js.</li>
	<li>Together with all UI assets of the app, the component is located in the webapp folder.</li>
	<li>The index.html file is located in the webapp folder if it is used productively.</li>
	<strong> Descriptor for Applications</strong>
	<li>The descriptor file is named manifest.json and located in the webapp folder.</li>
	<li>Use translatable strings for the title and the description of the app.</li>
	<strong> Margins and Paddings</strong>
	<li>Use the standard SAPUI5 CSS classes for the layout if possible.</li>
	<strong> Custom CSS and Theme Colors</strong>
	<li>Do not specify colors in custom CSS but use the standard theme-dependent classes instead.</li>
	<strong> Icons</strong>
	<li>Always use icon fonts rather than images wherever possible, as they are scalable without quality loss (vector graphics) and do not need to be loaded separately.</li>
	<strong> Data Types</strong>
	<li>Use Unicode escape sequences for special characters.</li>
	<strong> Expression Binding</strong>
	<li>Only use expression binding for trivial calculations.</li>
	<strong> Mock Server Configuration</strong>
	<li>The webapp/test folder contains non-productive code only.</li>
	<li>Mock data and the script to start the MockServer are stored in the webapp/localService folder.</li>
	<li>The script to start the MockServer is called mockserver.js.</li>
	<strong> Unit Test</strong>
	<li>All unit tests are placed in the webapp/test/unit folder of the app.</li>
	<li>The default naming convention for the test suite is testsuite.qunit.html and testsuite.qunit.js. When adding additional test suites, the naming must follow the pattern testsuite.<name>.qunit.html/testsuite.<name>.qunit.js.</li>
	<li>Test files referenced in the test suite end with .qunit.js.</li>
	<li>A unit test should be written for formatters, controller logic, and other individual functionality.</li>
	<li>All dependencies are replaced by stubs to test only the functionality in scope.</li>
	<strong> Unit Test with QUnit</strong>
	<li>All unit tests are placed in the webapp/test/unit folder of the app.</li>
	<li>The default naming convention for the test suite is testsuite.qunit.html and testsuite.qunit.js. When adding additional test suites, the naming must follow the pattern testsuite.<name>.qunit.html/testsuite.<name>.qunit.js.</li>
	<li>Test files referenced in the test suite end with .qunit.js.</li>
	<li>A unit test should be written for formatters, controller logic, and other individual functionality.</li>
	<li>All dependencies are replaced by stubs to test only the functionality in scope.</li>
	<strong> Integration Test with OPA</strong>
	<li>OPA tests are located in the webapp/test/integration folder of the application.</li>
	<li>Use page objects and journeys for structuring OPA tests.</li>
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
			We also give our app a title that will be displayed in the browser. Our hard-coded title can be overruled by the app, for example to show a title in the language of the user. The body part describes the layout of 
			the page. In our case, we simply display "Hello World" by using a div tag.
			</p>
		</li>
		<li> <strong> manifest.json </strong>
			<p>  
			All application-specific configuration options which we'll introduce in this tutorial will be added to this file.
			</p>
		</li>
	</ol></p>
<p>

 **_Info_** | **_Commands_** | **_Addition_** |
| --- | --- | --- |
| Command controller | **_CTRL+SHIFT+P_** | Commands |
| Show terminal | CTRL+' | Terminal |
| &nbsp; | &nbsp; | &nbsp; |
|     | **_npm init --yes_** | \-Create a package file and everything we need. |
|     | **_ui5 --help_** | In terminal: Shol all ui5 command in |
|     | **npm install --global @ui5/cli** | Install Fiori -- Test installation with **_ui5 --help_** |
|     | **npm init --yes** | Create a package file |
|     | **Ui5 init** | Create **yaml** file - Configuration and tooling file |
|     | Create manifest file | Create manifest.json file [Creating a Manifest File for Existing Apps - Documentation - Demo Kit - SAPUI5 SDK](https://ui5.sap.com/#/topic/3a9babace121497abea8f0ea66e156d9?q=create%20a%20description%20file%20for%20existing%20apps) |
|     | **_ui5 serve_** | Run on local machine return -- click on lint to access |
| &nbsp; | **_npm i -D @ui5/cli_** | install UI5 CLI - Inside node_modules |
| &nbsp; | **_ui5 use OpenUI5_** | &nbsp; |
| &nbsp; | **_ui5 add sap.ui.core sap.m themelib_sap_horizon_** | Add configuration into ui5.yaml file |
| &nbsp; | **_npm i -D ui5-middleware-simpleproxy_** | &nbsp;install this package as a new development dependency in your package.json. |
| &nbsp; | &nbsp; | &nbsp; |
