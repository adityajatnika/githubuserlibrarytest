# Github Users Library
This repository is made to publish libraries or dependencies that can be used to get data lists and Github user details on Android Studio projects.

## Advantage
✅ Simplify to get github user from API   
✅ Code Eficiency   
✅ No more define API Config    
✅ No more define API service   
✅ No more define Repository Data   

## Developer 
| Nama | NIM |
| --- | --- |
| Prasetya Naufal Rahmandita | 195150401111035 |
| Aditya Akhmad Dinan Jatnika | 195150401111025 |
| Mohammad Aditya Putra | 195150400111054 |
| Ronaldo Simatupang | 195150400111015 |
| Hendika Fashobiqul Galang F. | 195150400111024 |

## System Requirement (Recomendation / Tested)
- Android Studio Dolphin | 2021.3.1 Patch 1
- Kotlin Plugin Version : 213-1.7.20
- Android Gradle Plugin Version : 7.3.1
- Gradle Version : 7.4
- Compile SDK Version : 32 
- Java 8

## Tested on Devices
✅ Samsung Galaxy A03S   
✅ Samsung Galaxy A20S

## How to Use
#### Step 1 : Add the JitPack repository to your build file

```gradle
allprojects {
  repositories {
    ...
      maven { url 'https://jitpack.io' }
     }
  }    
```

#### Step 2 : Add the dependency
```gradle
dependencies {
  implementation 'com.github.adityajatnika:githubuserslibrary:Tag'
}
```

#### Step 3 : Choose The Feature
Example :
```

```
  
That's it! The first time you request a project JitPack checks out the code, builds it and serves the build artifacts (jar, aar).   
If the project doesn't have any GitHub Releases you can use the short commit hash or 'master-SNAPSHOT' as the version.

See also

[Documentation](https://docs.jitpack.io/)  
[Private Repositories](https://jitpack.io/private#auth)   
[Immutable Artifacts](https://docs.jitpack.io/#immutable-artifacts)   

## Features
### GetUsers
In this features provides you to get all data list data users in Github only
##### Syntax :
```kotlin
ApiGithubConfig.ApiService().getUsers(token)
```
##### Output :
| Name | Type | Variabel |
| --- | --- | --- |
| AvatarUrl User | String | avatarUrl |
| ID | Int | id |
| UserName | String | login |
### GetFollower
In this features provides you to get the number of follower based on the selected account
##### Syntax :
```kotlin
ApiGithubConfig.ApiService().getFollowers(token, query)
```
##### Output :
| Name | Type | Variabel |
| --- | --- | --- |
| Number of Follower | Int | followers |
### GetFollowing
In this features provides you to get the number of following based on the selected account 
##### Syntax :
```kotlin
ApiGithubConfig.ApiService().getFollowing(token, query)
```
##### Output :
| Name | Type | Variabel |
| --- | --- | --- |
| Number of Following | Int | following |
### GetDetailUser
In this features provides you to get the detail of account that you choose 
##### Syntax :
```kotlin
ApiGithubConfig.ApiService().getDetailUser(token, query)
```
##### Output :
| Name | Type | Variabel |
| --- | --- | --- |
| Number of Followers | Int | followers |
| AvatarUrl User | String | avatarUrl |
| Number of Following | Int | following |
| Name | String | name |
| Company | String | company |
| Location | String | location |
| ID | Int | id |
| Public Repositories | int | publicRepos |
| UserName | String | login |
## How it Works
## Resource
[Github API QUICKGUIDE](https://docs.github.com/en/get-started)
