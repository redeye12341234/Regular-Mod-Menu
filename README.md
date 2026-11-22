**INSTALLATION**

1. Add a folder somewhere on one of your drives
2. Place the .zip into that folder
3. Extract the .zip
4. Make sure you have **.NET 10 SDK** installed before continuing (If you do not install **.NET 10 SDK** the project will fail to build)
5. Open the extracted folder (named "Regular Mod Manager") in Terminal and run this command (right-click the folder and select Open in Terminal)

<img width="600" height="404" alt="{98BBF5B2-F762-4718-850B-2F34BC0C8EDA}" src="https://github.com/user-attachments/assets/dbf63550-ee20-4df2-98c4-db5f4c10e5db" />


```
dotnet restore; if ($?) { dotnet build -c Release }; if ($?) { Start-Process ".\\\\bin\\\\Release\\\\net10.0-windows\\\\Regular Mod Manager.exe" }
```



It should now build and launch the application automatically and you can close the terminal (the .exe will be located in: " Regular Mod Manager\\bin\\Release\\net10.0-windows\\Regular Mod Manager.exe ")



Enjoy!



**IMPORTANT**

All your games, mods and profiles are stored locally in your Windows LocalAppData folder (if you delete that folder your mods/profiles will be deleted)
This means you can uninstall and reinstall the application without losing your saved mods or profiles, as long as you don't manually delete its LocalAppData folder

The project itself doesn't connect to the internet. The installation process may require an internet connection to download .NET dependencies

The terminal command uses PowerShell 5.1 (to check if you're using 5.1 look at the top and it should say "Windows PowerShell 5.1") so do keep that in mind if you changed your default PowerShell settings!



**DISCLAIMER**
This project is developed entirely with ChatGPT



The project idea and concept were created by **RedEye**
