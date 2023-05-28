# config for startship-prompt
- Install startship prompt
`winget install --id Starship.Starship`

- Open Powershell as Administrator
- Delete ~/.config/startship.toml file if it exist
- Create .config folder and startship.toml file
`mkdir -p ~/.config`

- cd into the config directory
`cd ~/.config`

- Open CMD
- Create a symlink to ~/.config/startship.toml from startship-promp/startship.toml
`cd C:\Users\<USER>\.config`
`mklink starship.toml C:\SLinks\starship-prompt\starship.toml`