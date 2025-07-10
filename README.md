# PowerShell Profiles

A collection of customized PowerShell profiles designed to streamline systems administration tasks by providing commonly used functions and tools automatically loaded at startup.

## Overview

This repository contains PowerShell profiles that transform frequently used scripts into functions that are automatically available whenever you launch PowerShell. Instead of manually loading scripts or remembering complex commands, you can simply call these functions as needed.

## Installation

### Profile Locations

PowerShell profiles must be placed in specific locations depending on your PowerShell version and host application. Use `$profile | select *` to view the available profile paths on your system.

#### PowerShell 5.1
- **AllUsersAllHosts**: `C:\Windows\System32\WindowsPowerShell\v1.0\profile.ps1`
- **AllUsersCurrentHost**: `C:\Windows\System32\WindowsPowerShell\v1.0\Microsoft.PowerShell_profile.ps1`
- **CurrentUserAllHosts**: `C:\Users\<username>\Documents\WindowsPowerShell\profile.ps1`
- **CurrentUserCurrentHost**: `C:\Users\<username>\Documents\WindowsPowerShell\Microsoft.PowerShell_profile.ps1`

#### PowerShell ISE
- **AllUsersAllHosts**: `C:\Windows\System32\WindowsPowerShell\v1.0\profile.ps1`
- **AllUsersCurrentHost**: `C:\Windows\System32\WindowsPowerShell\v1.0\Microsoft.PowerShellISE_profile.ps1`
- **CurrentUserAllHosts**: `C:\Users\<username>\Documents\WindowsPowerShell\profile.ps1`
- **CurrentUserCurrentHost**: `C:\Users\<username>\Documents\WindowsPowerShell\Microsoft.PowerShellISE_profile.ps1`

#### PowerShell 7
- **AllUsersAllHosts**: `C:\Program Files\PowerShell\7\profile.ps1`
- **AllUsersCurrentHost**: `C:\Program Files\PowerShell\7\Microsoft.PowerShell_profile.ps1`
- **CurrentUserAllHosts**: `C:\Users\<username>\Documents\PowerShell\profile.ps1`
- **CurrentUserCurrentHost**: `C:\Users\<username>\Documents\PowerShell\Microsoft.PowerShell_profile.ps1`

#### Visual Studio Code
- **AllUsersAllHosts**: `C:\Program Files\PowerShell\7\profile.ps1`
- **AllUsersCurrentHost**: `C:\Program Files\PowerShell\7\Microsoft.VSCode_profile.ps1`
- **CurrentUserAllHosts**: `C:\Users\<username>\Documents\PowerShell\profile.ps1`
- **CurrentUserCurrentHost**: `C:\Users\<username>\Documents\PowerShell\Microsoft.VSCode_profile.ps1`

## Configuration

### Environment Customization

These profiles are currently configured for a homelab environment using domain naming conventions:
- `myhomelab.hv.lab` for Hyper-V based environments
- `myhomelab.vm.lab` for VMware based environments

To adapt them for your environment:

1. Search for all instances of `myhomelab.hv.lab` and `myhomelab.vm.lab` in the profile files
2. Replace with your domain name or environment-specific values
3. Review and adjust any other environment-specific settings as needed

### User-Specific Settings

⚠️ **Important**: Before using these profiles, you must customize the following placeholders:

- **Email addresses**: Replace `user@example.com` with your actual email address
- **Usernames**: Replace `uzrg` with your actual username or identifier
- **Repository URLs**: Update any hardcoded repository URLs to match your repositories

These placeholders are used throughout the profiles for Git configuration, SSH setup, and other user-specific operations.

### Getting Started

1. Clone this repository
2. Choose the appropriate profile file for your PowerShell version and use case
3. **Customize user-specific settings** (emails, usernames, repository URLs)
4. Customize domain and environment-specific settings
5. Copy the profile to the correct location (create directories if they don't exist)
6. Restart PowerShell to load the new profile

## Contributing

Contributions are welcome! Please feel free to:
- Submit improvements and enhancements
- Report issues or bugs
- Suggest new features or functions
- Share your own useful administration functions

## Support

Provided AS IS.

---

*These profiles are designed to make PowerShell administration more efficient by providing instant access to commonly used functions and tools.*
