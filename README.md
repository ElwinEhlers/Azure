# Azure
#How to see my network. IP test prepair peerings. 
<br>
Azure Cloud Shell
```html
az network vnet list --query '[].{"Region": location, "vNet": name, "CIDR": addressSpace.addressPrefixes[0]}' --output table
```
|Region              |VNet                |CIDR            |
|------------------  |  ----------------  |  ------------  |
|germanywestcentral  |ahoi-hub-vnet       |10.80.0.0/16    |
|germanywestcentral  |ahoi-spoke1-vnet    |10.81.0.0/16    |
|germanywestcentral  |ahoi-spoke2-vnet    |10.82.0.0/16    |
<br>
https://learn.microsoft.com/en-us/azure/virtual-network/virtual-network-peering-overview
