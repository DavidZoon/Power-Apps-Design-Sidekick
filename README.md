# Power-Apps-Design-Sidekick
### Theming templates for Power Apps Canvas apps, compatible with Creator Kit

### Requirements : Install Creator Kit Core first  : https://github.com/microsoft/powercat-creator-kit Version 1.0.20230118.1 or above

Creator kit is required to use the Theme Designer, but you can create themes for app without Creator Kit Compenents.

# What's is this solution ?

- Theme Designer application : To create custom themes
- 3 Template apps with custom theme variables prebuilt
- Component library with 2 Theme selectors

## Theme Designer : 

### View Themes :
![image](https://user-images.githubusercontent.com/125589668/220306221-a57df476-3244-4dbe-b16c-eaeb5f2e0cc9.png)

### Design Color theme (Same as creator Kit) :
![image](https://user-images.githubusercontent.com/125589668/220306418-2401843b-97d2-4bd4-9184-c789a4947daf.png)

### Design Format Theme :
![image](https://user-images.githubusercontent.com/125589668/220409394-54bc706d-eec5-43cd-bc14-5d1b2be00d36.png)

### Paste and copy code :
![image](https://user-images.githubusercontent.com/125589668/220307800-0d628387-ea69-499e-89d3-7c602cb5d495.png)
(Actual Color Theme and Format Theme will be default values)

### Preview Themes :
![msedge_KHg1PKafBL](https://user-images.githubusercontent.com/125589668/220310546-bda02d09-0ce0-4890-8edb-a6b3eba52a82.gif)

## Use Canvas Templates :

### 1. From your Solution, add an existing app :
![image](https://user-images.githubusercontent.com/125589668/220410020-5065ec2e-bd24-4e9c-8e50-da46aadc628e.png)
### 2. Select the app template and click "Add" :
![image](https://user-images.githubusercontent.com/125589668/220410844-631b3359-201b-418a-bf84-8ff52b827e4c.png)
### 3. Open app in editor and click "Save as" and set your app name :
![image](https://user-images.githubusercontent.com/125589668/220411136-61f7fb44-55f4-4cad-aa44-b13b13a5881b.png)    ![image](https://user-images.githubusercontent.com/125589668/220411481-42bff39a-7182-4e80-8417-3a6cb2e9d59d.png)
### 4. Go back to you solution and remove the template app from solution :
![image](https://user-images.githubusercontent.com/125589668/220411846-2e3a038a-076f-45bb-88fa-b50251e0aeb8.png)

## Use Theme Picker Component :
### Better copy and paste the compoenent from you Canvas Template
### If you want to import the component from library, you need to :
- customize component
- Turn "Access app scope" On in component parameters
- In app settings, enable "Enhaced Component properties"
- In app, set the component custom properties to : 
  - ColorTheme :
  > AppTheme
  - FormatTheme :
  > AppFormat
  - OnSelectThemeColor :
  > Set(AppTheme,Self.SelectedThemeColor);Set(AppThemeJson,JSON(AppTheme,JSONFormat.IndentFour));Set(AppThemeJson,JSON(AppTheme,JSONFormat.IndentFour))
  - OnSelectThemeFormat :
  > Set(AppFormat,Self.SelectedThemeFormat)

