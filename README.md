# git.config
My git config

To edit your gitconfig globally:

```bash
git config --global --edit
```

---

I love VSCode so before I edit my gitconfig I usually do:

```bash
git config --global core.editor "code -w"
```

To set my git editor to VSCode

---

### Windows pain (ps not WSL):

Run the following to have ssh-agent working (and start automatically)  
In powershell with admin priveledge
```powsershell
Get-Service ssh-agent | Set-Service -StartupType Automatic
```

Tell git to use the windows version of ssh as well (why we need to do this windows?)
```
git config --global core.sshCommand "'C:\Windows\System32\OpenSSH\ssh.exe'"
```

PS - Don't forget to add the ssh key
```
ssh-add "C:\Path\to\your\ssh\key"
```
