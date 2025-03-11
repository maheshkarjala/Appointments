<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>
  
<style>
        .slds-visual-picker_vertical .slds-visual-picker__figure {
            height: inherit !important;
        }

        .runtime_appointmentbookingFlowLocation .slds-visual-picker_vertical {
            display: inline-flex !important;
        }
</style>

  <script src="https://lucid-3f-dev-ed.develop.my.site.com/lightning/lightning.out.js"></script>

  <script>
    $Lightning.use("runtime_appointmentbooking:lightningOutGuest",
        function() {                  // Callback once framework and app load
            $Lightning.createComponent(
                "lightning:flow",    // top-level component of your app
                { },    // attributes to set on the component when created
                "lexcontainer",    // the DOM location to insert the component
                function(component) {            // API name of the Flow
                    component.startFlow("runtime_appointmentbooking__Guest_Flow");
                }
            );
        },    'https://lucid-3f-dev-ed.develop.my.site.com'  // Site endpoint
    );
</script>
  <div id="lexcontainer">
<p>Invoke the Lightning Component specified in the Script.</p>
</div>
</body>
</html>
