<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tableau Visualization</title>
    <!-- Include the Tableau JavaScript API -->
    <script type="text/javascript" src="https://public.tableau.com/javascripts/api/viz_v1.js"></script>
</head>
<body>
    <!-- Placeholder for Tableau visualization -->
    <div id="tableauViz"></div>

    <!-- JavaScript to embed Tableau visualization -->
    <script type="text/javascript">
        // Function to embed Tableau visualization
        function initViz() {
            var containerDiv = document.getElementById("tableauViz");
            var url = "https://public.tableau.com/views/YourVisualization";
            var options = {
                width: "100%",
                height: "600px",
                hideTabs: true,
                hideToolbar: true
            };
            var viz = new tableau.Viz(containerDiv, url, options);
        }

        // Call the function to embed the visualization when the page loads
        document.addEventListener("DOMContentLoaded", initViz);
    </script>
</body>
</html>
