API overview
############


.. raw:: html

    <div id="swagger-ui"></div>

    <script src='../_static/js/swagger-ui-bundle-3.18.3.js' type='text/javascript'></script>
    <script src='../_static/js/swagger-ui-standalone-preset-3.18.3.js' type='text/javascript'></script>
    <script>
        function HideTopbarPlugin() {
          // this plugin overrides the Topbar component to return nothing
          return {
            components: {
              Topbar: function() { return null }
            }
          }
        }

        window.onload = function() {
            const ui = SwaggerUIBundle({
                "dom_id": "#swagger-ui",
                validatorUrl: null,
                urls: [
                    {url: "../_static/nuts-consent-bridge.yaml", name: "consent-bridge"},
                    {url: "../_static/nuts-fhir-validation.yaml", name: "fhir-validation"},
                    {url: "../_static/nuts-registry.yaml", name: "nuts-registry"},
                    {url: "../_static/nuts-service-crypto.yaml", name: "crypto"}
                    ],
                presets: [
                    SwaggerUIBundle.presets.apis,
                    SwaggerUIStandalonePreset,
                    HideTopbarPlugin
                ],
                layout: "StandaloneLayout"
            });

            window.ui = ui
        }

    </script>