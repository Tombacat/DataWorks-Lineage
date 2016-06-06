# DataWorks-Lineage
There are three steps to take:
1. Load the zip file with
https://<your IIS>:<your IIS port>/ibm/iis/igc-rest/v1/bundles/
This zip file is the bundle and can be changed by unzipping, editing the asset_type_descriptor.xml. Be aware of the icons sizes (16x16 and 32x32). For more info please read https://is-server:9445/ibm/iis/igc-rest/v1/bundles/
2. After successful upload of the bundle, please use DataWorks-assetdoc.xml to load asset instances. Be aware that this is a specific sample and needs adjustment to your actual case. Load the xml data with
https://<your IIS>:<your IIS port>/ibm/iis/igc-rest/v1/bundles/assets
3. Finally stitch the instances together. Use DataWork-design-flow.doc.xml as reference and upload via
https://<your IIS>:<your IIS port>/ibm/iis/igc-rest/v1/flows/upload
