# WINDOWS INSTRUCTIONS


### How to create variable file

You need to create this file before run the command to build your template.

```
{
    "vcenter-user": "vCenter-User",
    "vcenter-password": "YourPassword",
    "winadmin-username": "Administrator",
    "winadmin-password": "YourPassword"
}
```

Save this file in the same local as your **windows2019.json** file.

###  Type the command below

```
packer build -var-file="variables-vars.json windows2019.json
```

### Variables

Username and Password variables are inside the file **variables-vars.json**

### Creating Unattend File

Download and Install Windows ADK

https://go.microsoft.com/fwlink/?linkid=2120254

Import **autounattend.xml** file and make the changes or create your own file following the intructions: https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/update-windows-settings-and-scripts-create-your-own-answer-file-sxs

