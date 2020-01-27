Download the OVF Tool
--------------------------

**1)** Go to [OVF Tool](https://code.vmware.com/web/tool/4.3.0/ovf) and click on the Download button for `4.3.0`

**2)** When I downloaded the tool, it was placed here

```
Austins-MacBook-Pro-2:VMware OVF Tool Austin$ pwd
/Applications/VMware OVF Tool
```

Using the OVF Tool
--------------------------

**1)** In your terminal, go to the OVF download location

**2)** For me, I have a folder in my `Documents` folder that contains the VM images:

```
Austins-MacBook-Pro-2:Virtual Machines.localized Austin$ pwd
/Users/Austin/Documents/Virtual Machines.localized
```

**3)** From the terminal where you have the OVF Tool in, you can enter the following to create the OVA image

```
Austins-MacBook-Pro-2:VMware OVF Tool Austin$ ./ovftool /Users/Austin/Documents/Virtual\ Machines.localized/Blockchain\ 1.4.3.vmwarevm/Blockchain\ 1.4.3.vmx /Users/Austin/Documents/Virtual\ Machines.localized/blockchain143.ova
```

Basically the syntax is: 

```
./ovftool <location of your VM image with the .vmx ending> <location with the .ova ending>
```

**4)** Expectated output:

```
Opening VMX source: /Users/Austin/Documents/Virtual Machines.localized/Blockchain 1.4.3.vmwarevm/Blockchain 1.4.3.vmx
Opening OVA target: /Users/Austin/Documents/Virtual Machines.localized/blockchain143.ova
Writing OVA package: /Users/Austin/Documents/Virtual Machines.localized/blockchain143.ova
Transfer Completed                    
Completed successfully
```

It takes some time to complete, but it was finished in ~5 minutes. 

Useful Resources
---------------

Video of someone doing what you're looking to do: 

[Using OVF Tools](https://www.youtube.com/watch?v=3uBTGUTrOfM&t=186s)

Skytap Docs for using the OVF Tool:

[Documentation](https://help.skytap.com/Using_OVF_Converter_Tool.html)
