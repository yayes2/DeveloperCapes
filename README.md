DonorCapesAPI
=============

##Version: 1.1

A Minecraft API for adding Donor/Tester only capes!
Use this to add tester or donor only capes to your mod!


#Usage:
For now, make a new method in your CommonProxy and ClientProxy classes called capesInit or something (Or just use your registerRenderInformation sort of method). Leave the Common one blank and put this in the ClientProxy one. We do this so it only executes on client side. Put this in it.

```java
DonorCapesAPI.init(*CAPES TXT*, 
	*DONOR CAPE URL*,
	*TESTER CAPE URL*);
```

Then in your preInit or init method in your main mod class just call the capesInit method.

The capes txt is a text file hosted on a server (or Dropbox) that has all the users you want to have capes in. The layout looks like this
```
donor: username1
donor: username2
tester: username3
tester: username4
```
Make sure to have the space between ':' and the username.

The cape image files are 22x17, and should be of the PNG format. Host them on a server or Dropbox. Maybe I'll add client hosted capes.
