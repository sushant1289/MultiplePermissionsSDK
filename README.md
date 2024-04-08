### This is a multiple permission request SDK using Jetpack compose ###
- Add the JitPack repository to your build file Add it in your root build.gradle at the end of repositories:
```
dependencyResolutionManagement {
		repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
		repositories {
			mavenCentral()
			maven { url 'https://jitpack.io' }
		}
	}
```

- Add the dependency
```
dependencies {
	        implementation 'com.github.sushant1289:MultiplePermissionsSDK:Tag'
	}
```

- The Latest Release is 1.1

- To use it's functionality:
   - You have to include the permissions which you want to ask and enable in the app.
   - Then go to the main activity and create an array of Permissons like this:
     
     ```
     private val permissionsToRequest = arrayOf(
        Manifest.permission.CAMERA,
        Manifest.permission.RECORD_AUDIO,
        Manifest.permission.ACCESS_COARSE_LOCATION,
        Manifest.permission.ACCESS_FINE_LOCATION,
        Manifest.permission.CALL_PHONE
    )
  ```
- Then inside the setContent block add This below line:

  ```
  PermissionProvider(
                        activity = this,
                        permissionsToRequest = permissionsToRequest
                    )
  ```
And you are all set to use this SDK

![image](https://github.com/sushant1289/MultiplePermissionsSDK/assets/165392691/c2033ee6-1dc7-4e0d-9958-dc0650cc1f00)

