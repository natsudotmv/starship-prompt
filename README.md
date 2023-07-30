# config for startship-prompt
- Install startship prompt
```powershell
winget install --id Starship.Starship
```

*Note: Below instructions assumes current user have admin privileges. If you are using another user as admin, you have to type the path eg:(C:\\Users\\%username%\\.config)*

- Open Powershell as Administrator
- Delete ~/.config/startship.toml file if it exist
- Create .config folder and startship.toml file
```powershell
mkdir -p ~/.config
```

- cd into the SLinks directory
```powershell
cd C:\SLinks
git clone https://github.com/natsudotmv/starship-prompt.git
```

- Open CMD as Administrator
- Create a symlink to ~/.config/startship.toml from startship-promp/startship.toml
```cmd
cd %userprofile%\.config
```
```cmd
mklink starship.toml C:\SLinks\starship-prompt\starship.toml
```