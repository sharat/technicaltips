You might bump in to this problem if you're signing your binaries 

`SignTool Error: Signtool requires CAPICOM version 2.1.0.1`


```
1. Download the latest CAPICOM "Platform SDK Redistributable" here. 
2. Run the downloaded [capicom_dc_sdk.msi](http://www.microsoft.com/en-us/download/details.aspx?id=25281) file. 
3. Register capicom.dll as follows.

regsvr32 "C:\Program Files (x86)\Microsoft CAPICOM 2.1.0.2 SDK\Lib\X86\CapiCom.dll"


```

The installation might vary depends on your operating system (x86/x64) and version of the software being installed.
