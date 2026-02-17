# ZG Admin - Update Logs

## Version 2.1.0 - February 17, 2026
### 🎉 New Features
- Added persistent data storage with Replit Database
- All user data now persists across deployments
- New admin endpoints to view database (/admin/data, /admin/stats, /admin/export)

### 🔧 Improvements
- Fixed key validation system - keys now persist in database
- Improved /assign and /remove commands with timeout prevention
- Keys are now saved immediately when generated

### 🐛 Bug Fixes
- Fixed "Key not found" error - keys now persist across restarts
- Fixed "Application did not respond" timeout on /assign command
- Fixed port binding issue for Replit deployments

### 📊 Database Features
- User connections persist forever
- Booster claims saved to database
- Staff roles saved to database
- Active keys saved to database
- View data in Replit Database panel or via /admin/data

---

## Version 2.0.0 - February 16, 2026
### 🎉 Major Update - Login System
- New /login and /logout commands
- One-to-one Discord ↔ Roblox account mapping
- Users must login before claiming roles
- /claim now requires no arguments (uses logged-in account)
- /assign now uses Discord users instead of Roblox usernames

### 🔧 Command Changes
- /login <roblox_username> - Connect your Discord to Roblox
- /logout - Disconnect your accounts
- /claim - Claim booster tag (requires login + booster role)
- /unclaim - Remove booster claim
- /assign <role> <discord_user> - Owner assigns staff roles
- /remove <discord_user> - Owner removes staff roles

### 🛡️ Security Improvements
- Account locking prevents account stealing
- One Discord account = One Roblox account
- Users must /logout to switch accounts
- Prevents duplicate claims

---

## Version 1.5.0 - February 15, 2026
### 🎉 New Features
- Added keep-alive system (re-posts messages every hour)
- Auto-delete old messages on startup
- Rich Presence status

### 🔧 Improvements
- Mobile-optimized Roblox script (92% less CPU, 75% less battery)
- PC blocking on mobile script
- Better key validation messages

### 🐛 Bug Fixes
- Fixed message posting issues
- Fixed key expiration cleanup

---

## Version 1.0.0 - February 14, 2026
### 🎉 Initial Release
- Discord bot with key system
- Premium keys support
- Booster role claims
- Staff role assignments (Head of Staff, Admin, Moderator)
- Roblox script integration
- 24-hour free keys
- Private DM verification
