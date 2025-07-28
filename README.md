1. Clone the project from the Git repository.
 
2. Update Namespace (Optional):
   Change the namespace if needed (e.g: rits.custom.pod.examples.custompodpluginexamples).
 
3. Inside the webapp folder, the following three plugins are available:
 
        custompodpluginexamples – Main plugin that acts as a container for the other two.
 
        exampleWip – This plugin will graphically display work centers along with the active orders and SFC (Shop Floor Control) details.
 
 
4. Build the mta.yaml using your preferred method:
 
        Run mbt build, or
 
        Right-click the project and choose “Build MTA Project”.
 
5. Deploy the generated .mtar file to your Cloud Foundry space.
 
6. After deployment, get the application URL.
 
        Note the plugin path from index.html (e.g., /custompodpluginexamples) and the namespace (e.g., rits.custom.pod.examples.custompodpluginexamples).

 
7. Register the Plugin in SAP DMC

        Go to Manage Service Registry → UI Extensions tab.
 
        Create a new UI Extension entry:
 
        Use the plugin URL in the URL Field
		
		path in the path field
		
		Format the namespace using slashes (e.g., rits/custom/pod/examples/custompodpluginexamples).
 
        Enable the status and click Create.
 
8. Verify Plugin in POD Designer
	    After registration, the plugins should be visible in the POD Designer.

9. Use the Plugin in POD Designer Drag and drop exampleWip onto a relevant POD layout such as WorkCenter or Operation.

10. You can now view the deployed plugin within your selected POD.
