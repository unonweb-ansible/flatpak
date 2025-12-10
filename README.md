# NOTES

Per-user installations are only available to the user that installed them, while system-wide installations are available to all users on the system
System-wide installations can be updated by any user with administrator privileges

# CLI

**Add remote repo**:
`flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo`

**Delete remote repo**:
`flatpak remote-delete flathub`
(Requires all associated apps to be uninstalled!)

**Add only verified apps to your local repository:**
`flatpak remote-add --if-not-exists --subset=verified flathub-verified https://flathub.org/repo/flathub.flatpakrepo`

**Remove a subset and return to the unfiltered repository:**
`flatpak remote-modify --subset= flathub`