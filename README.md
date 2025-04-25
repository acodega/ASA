# ASA - Apple Screenshots for Admins

This GitHub repo is a community-maintained collection of high-quality, version-specific Apple platform UI screenshots for Apple IT professionals.

The goal is to provide a consistent, reliable reference for:
- Setup Assistant screens
- System Settings / System Preferences panels
- Security & Privacy prompts (TCC)
- MDM-related dialog boxes

This project exists to save time, reduce guesswork, and provide a dependable visual source of truth—so Apple admins don’t have to rely on random Google Image results or take screenshots from scratch.

## We welcome community contributions!
Our folder structure:
```
platform_feature/
├── en-US/
├── en-GB/
│   ├── macos_version_name-of-screenshot.png
│   └── (...)
└── (...)
```

To Submit a Pull Request:
1. Fork the repo and create a new branch.
2. Add your screenshots to the appropriate folder. (To begin, we're open to folder suggestions)
3. Screenshots should be as generic as possible. Standard resolution, light mode, default wallpaper, no unique menu bar apps or dock customization. In general, we recommend full screen screenshots. This lets others crop as they need, rather then being limited by an isolated dialog box/window screenshot.
4. Open a PR. Make sure your PR only adds the screenshots you are offering, and does not edit or delete any other files.
5. If you're adding a new UI change, document it briefly in the PR description. Example: What's the new change you're screenshoting, and what OS version did the change you're screenshoting show up?

### Filename Breakdown

| Field           | Description                                             | Example                          |
|----------------|---------------------------------------------------------|----------------------------------|
| `platform`| macOS, iOS etc.  | `mac`, `iOS`, `iPadOS`           |
| `version`| OS version, use full number if needed (e.g. `15.4`)  | `15.4`, `14.0`, `13.6`           |
| `area`         | Broad UI category or location                           | `setup-assistant`, `tcc`, `system-settings`, `mdm` |
| `screen`       | Specific screen, setting, or prompt                     | `location-services`, `passkeys`, `screen-recording` |
| `context`      | *(Optional)* App name, condition, or variation          | `Restricted`, `disabled`, `MDM-managed` |

- Use **underscore (`_`)** to separate each part.
- Use **kebab-case** (lowercase, hyphenated) inside each part.
- Use `.png` format for all files.

#### Examples

```mac_15.4_setup-assistant_passkeys.png
mac_14.0_tcc_screen-recording_terminal.png
mac_15.0_tcc_local-network_google-chrome.png
mac_13.6_system-settings_login-items.png
mac_15.0_mdm_remote-management.png
mac_15.4_system-settings_profiles.png
