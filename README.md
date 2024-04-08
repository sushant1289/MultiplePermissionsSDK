### This is a multiple permission request SDK ###
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
