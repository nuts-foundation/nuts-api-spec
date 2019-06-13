.. _nuts-node-rpc-spec:

Nuts API's
==========

This documentation site contains all API definitions used in intra- and inter-node communication.

Back to main documentation: :ref:`nuts-documentation`

.. raw:: html

    <div id="swagger-ui"></div>

    <script src='_static/js/swagger-ui-bundle-3.18.3.js' type='text/javascript'></script>
    <script src='_static/js/swagger-ui-standalone-preset-3.18.3.js' type='text/javascript'></script>
    <script>
        window.onload = function() {
            const ui = SwaggerUIBundle({
                "dom_id": "#swagger-ui",
                urls: [
                    {url: "_static/nuts-consent-bridge.yaml", name: "consent-bridge"},
                    {url: "_static/nuts-consent-logic.yaml", name: "consent-logic"},
                    {url: "_static/nuts-fhir-validation.yaml", name: "fhir-validation"},
                    {url: "_static/nuts-registry.yaml", name: "nuts-registry"},
                    {url: "_static/nuts-service-crypto.yaml", name: "crypto"},
                    {url: "_static/nuts-auth.yaml", name: "auth"},
                    {url: "_static/nuts-consent-store.yaml", name: "consent-store"},
                    ],
                presets: [
                    SwaggerUIBundle.presets.apis,
                    SwaggerUIStandalonePreset
                ],
                layout: "StandaloneLayout"
            });

            window.ui = ui
        }

    </script>
