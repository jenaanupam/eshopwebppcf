This will use inmemorycache to store data.
So might not work properly when deployed on multiple containers. keep container count =1

cd F:\git\pcf working projects\eshopwebppcf\eshopweb\eShopOnWeb\src\WebRazorPages

dotnet publish --configuration release  -f netcoreapp2.0 -r ubuntu.14.04-x64

cf push -f manifest.yml -p bin/release/netcoreapp2.0/ubuntu.14.04-x64/publish