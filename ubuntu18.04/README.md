# UBUNTU INSTRUCTIONS

### Password Secure Generate
```
printf "meupassword123" | mkpasswd -s -m md5

$1$MtWS4R4E$rcpocKlLwwP7rWuGO09kT/
```
###  Type the command below
```
packer build -var 'vcenter_key=yourpassword' -var 'ssh_user=chl' -var 'ssh_pass=meupassword123' ubuntu1804.json
```
