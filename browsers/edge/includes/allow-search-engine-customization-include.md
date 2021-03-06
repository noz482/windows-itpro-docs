<!-- ## Allow search engine customization -->
>*Supported versions: Microsoft Edge on Windows 10, version 1703 or later*<br>
>*Default setting:  Enabled or not configured (Allowed)*

[!INCLUDE [allow-search-engine-customization-shortdesc](../shortdesc/allow-search-engine-customization-shortdesc.md)]

### Supported values

|Group Policy  |MDM |Registry |Description |Most restricted |
|---|:---:|:---:|---|:---:|
|Disabled |0 |0 |Prevented/not allowed |![Most restricted value](../images/check-gn.png) |
|Enabled or not configured<br>**(default)** |1 |1 |Allowed | |
---

### Configuration options

For more details about configuring the search engine, see [Search engine customization](../group-policies/search-engine-customization-gp.md).

### ADMX info and settings

##### ADMX info
- **GP English name:** Allow search engine customization
- **GP name:** AllowSearchEngineCustomization
- **GP path:** Windows Components/Microsoft Edge
- **GP ADMX file name:** MicrosoftEdge.admx

#### MDM settings
- **MDM name:** Browser/[AllowSearchEngineCustomization](https://docs.microsoft.com/en-us/windows/client-management/mdm/policy-csp-browser#browser-allowsearchenginecustomization)
- **Supported devices:** Desktop and Mobile
- **URI full path:** ./Vendor/MSFT/Policy/Config/Browser/AllowSearchEngineCustomization
- **Data type:** Integer


#### Registry settings
- **Path:** HLKM\\Software\\Policies\\Microsoft\\MicrosoftEdge\\Protected
- **Value name:** AllowSearchEngineCustomization
- **Value type:** REG_DWORD


### Related policies

- [Set default search engine](../available-policies.md#set-default-search-engine): [!INCLUDE [set-default-search-engine-shortdesc](../shortdesc/set-default-search-engine-shortdesc.md)]

- [Configure additional search engines](../available-policies.md#configure-additional-search-engines): [!INCLUDE [configure-additional-search-engines-shortdesc](../shortdesc/configure-additional-search-engines-shortdesc.md)]

### Related topics

- [!INCLUDE [man-connections-win-comp-services-shortdesc-include](man-connections-win-comp-services-shortdesc-include.md)]

- [!INCLUDE [search-provider-discovery-shortdesc-include](search-provider-discovery-shortdesc-include.md)]

<hr>