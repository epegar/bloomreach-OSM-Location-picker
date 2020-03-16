# Bloomreach OSM Location picker
This project is a Bloomreach [OpenUI extension](https://documentation.bloomreach.com/library/concepts/open-ui/introduction.html). The purpose of the extension is to make it easy for editors to pick locations. In this case by using a map and a search bar.

![screenshot](./images/screenshot_dialog.png?raw=true)

The extension uses OpenStreetMaps because there isn't any kind of quota or accout needed, so it's easier to set up.

The demo directory contains an archetype where the pluin has been included. 

## Steps to run the demo:

1. Start Bloomreach: go to the demo directory and use `mvn clean verify && mvn -P cargo.run`.
2. Start the extension: the easiest way to load the extension is using the included scripts `docker-build.sh` and `docker-run.sh`.

## How to setup the extension in your project?

1. You'll have to define the extension under `/hippo:configuration/hippo:frontend/cms/ui-extensions`. In this case, if you take a look at the demo, you'll find the following node: `/hippo:configuration/hippo:frontend/cms/ui-extensions/locationPicker`.
![screenshot](./images/Screenshot_console.png?raw=true)
2. [Add this extension to a document type](https://documentation.bloomreach.com/library/concepts/open-ui/configure-a-document-field-extension.html). You can alse check the only document type defined on the demo. 
