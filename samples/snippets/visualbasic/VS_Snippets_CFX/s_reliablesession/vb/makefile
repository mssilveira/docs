all: service.exe client.exe
 
service.exe: service.vb 
 vbc /t:library service.vb /r:System.ServiceModel.dll /libpath:"c:\whidbey\assemblies"
 
client.exe: client.vb generatedProxy.vb
 vbc /t:exe client.vb generatedProxy.vb /r:System.ServiceModel.dll /libpath:"c:\whidbey\assemblies"
