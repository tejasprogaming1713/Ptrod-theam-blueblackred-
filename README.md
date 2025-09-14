# Neon Theme for Pterodactyl Panel

This is a custom **neon-styled theme** for the Pterodactyl Game Panel.  
It features a **red + blue neon geometric background**, glowing buttons, and a modern dark UI for your panel.

## ✨ Features
- 🔥 Neon **red + blue** background (customizable)  
- 🎨 Custom **login page styling** with glowing effects  
- 🌙 Dark transparent containers for better contrast  
- ⚡ Animated button hover effects  
- 📂 Organized structure for easy updates and GitHub syncing  

## 📂 Repo Structure
```
panel-theme/
├── README.md              # Setup instructions
├── public/
│   └── themes/neon/       # Theme assets
│       ├── bg.jpg         # Neon background
│       └── custom.css     # CSS overrides
├── resources/
│   └── views/layouts/     # Blade template override
│       └── app.blade.php
```

## 🚀 Installation
1. Clone the repo into your panel:
   ```bash
   cd /var/www/pterodactyl
   git clone https://github.com/YOURNAME/panel-theme.git themes/neon
   ```

2. Copy files into your panel:
   ```bash
   cp -r themes/neon/resources/views/layouts/* resources/views/layouts/
   cp -r themes/neon/public/themes/neon public/themes/
   ```

3. Rebuild the frontend:
   ```bash
   yarn build:production
   php artisan view:clear
   php artisan cache:clear
   ```

4. Refresh the panel — your **Neon Theme** is active 🎉
