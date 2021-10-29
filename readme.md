

https://github.com/Azure/azure-iot-explorer/releases


https://apps.azureiotcentral.com/build/new/custom

https://hub.docker.com/_/microsoft-azureiotedge-testing-utility

https://github.com/Azure

https://github.com/Azure/azure-iot-sdk-python


Device models repository
https://docs.microsoft.com/en-us/azure/iot-develop/concepts-model-repository


plug-and-play

https://docs.microsoft.com/en-us/azure/iot-develop/concepts-developer-guide-device?pivots=programming-language-python


https://github.com/Azure/opendigitaltwins-dtdl


scopeID="0ne0040D798"
deviceID="23usjxkypgy"


az deployment group create \
  --resource-group silo_iot_vqc \
  --template-uri 
  --parameters scopeID="0ne0040D798" \
  --parameters deviceID="23usjxkypgy" \
  --parameters deviceKey="9aP5lOv5Z2iIJ5m8Api5Q00Hfhy0pbajc7BENVYZAUw="


az deployment group create \
  --name edgeModuleVM \
  --resource-group [sandbox resource group name] \
  --template-uri https://raw.githubusercontent.com/Azure-Samples/iot-central-docs-samples/master/edge-vm-deploy/edgeModuleVMDeploy.json \
  --parameters dnsLabelPrefix="$APP_NAME" \
  --parameters adminUsername="AzureUser" \
  --parameters adminPassword="$VM_PASSWORD" \
  --parameters scopeId="" \
  --parameters deviceId="store-001" \
  --parameters deviceKey="$DEVICE_KEY"
