_AospExtended for Moto G Devices_
------------------------------------

the local manifests:

	$ repo init -u git://github.com/AospExtended/manifest.git -b 8.1.x
	$ git clone https://github.com/falcon-oreo/local_manifest -b AospExtended .repo/local_manifests

Then sync up with this command:

	$ repo sync -c --force-sync --no-clone-bundle --no-tags
	

-------------
 
_Building from source_
---------------

	$ export USE_CCACHE=1
	$ prebuilts/misc/linux-x86/ccache/ccache -M 50G
	$ . build/envsetup.sh
	$ lunch aosp_device_codename-userdebug
	$ mka aex -jx

-------------
 
_Credits:_
---------------
@luk1337
@luca020400
@RahifM
@RenanQueiroz
@Andersonmendes2016
@Team LineageOS
@And More people
