# 📱 Mobile Coding Tools Guide

**Learning to code on your phone?** You're in the right place! Here are the best free tools for coding on mobile devices.

---

## 🌟 Best Mobile Code Editors

### 1. Termux (Android) ⭐ RECOMMENDED
**Free | Offline | Full Linux Terminal**

Termux turns your Android phone into a complete development environment.

**Download:** [F-Droid](https://f-droid.org/packages/com.termux/) (recommended) or Google Play

**What you can do:**
- Write and run C, C++, Python, JavaScript, Assembly
- Install GCC, Clang, Node.js, Python
- Use Git for version control
- SSH to remote servers
- Fully offline once installed

**Quick Setup:**
```bash
# Update packages
pkg update && pkg upgrade

# Install essential tools
pkg install git vim nano python clang nodejs

# Install C/C++ compiler
pkg install build-essential

# Test your setup
gcc --version
python --version
```

**Learn more:** [Termux Wiki](https://wiki.termux.com/)

---

### 2. Spck Editor (Android & iOS)
**Free | Web Development Focused**

Great for HTML, CSS, JavaScript, and Node.js development.

**Download:** 
- [Google Play](https://play.google.com/store/apps/details?id=io.spck)
- [App Store](https://apps.apple.com/app/spck-editor/id1436320289)

**Features:**
- Live preview for web projects
- Git integration
- Code completion
- Emmet support

---

### 3. Acode (Android)
**Free | Lightweight | Offline**

Powerful code editor with syntax highlighting for 100+ languages.

**Download:** [Google Play](https://play.google.com/store/apps/details?id=com.foxdebug.acode)

**Features:**
- Syntax highlighting (C, C++, JS, Python, Assembly)
- File manager
- Git support
- Customizable themes

---

### 4. Dcoder (Android & iOS)
**Free tier available | Online compiler**

Mobile IDE with built-in compilers for many languages.

**Download:**
- [Google Play](https://play.google.com/store/apps/details?id=com.paprbit.dcoder)
- [App Store](https://apps.apple.com/app/dcoder-mobile-coding-ide/id1192875308)

**Languages supported:**
- C, C++, C#, Java, Python, JavaScript, Assembly (limited)

**Note:** Requires internet connection for compilation.

---

### 5. GitHub Mobile App
**Free | Essential for learning from this repository**

Access all lessons, browse code, and track your progress.

**Download:**
- [Google Play](https://play.google.com/store/apps/details?id=com.github.android)
- [App Store](https://apps.apple.com/app/github/id1477376905)

**Perfect for:**
- Reading lessons on the go
- Copying code examples
- Saving repositories offline
- Contributing back to the project

---

## 🖥️ Online Compilers & IDEs (Any Device)

### Replit
**Website:** [replit.com](https://replit.com)
- Supports C, C++, C#, JavaScript, Python, Assembly
- Free tier available
- Can work on mobile browsers
- Collaborative features

### OnlineGDB
**Website:** [onlinegdb.com](https://onlinegdb.com)
- Simple, fast online compiler
- Supports C, C++, Assembly, Python, JavaScript
- Debugger included
- Mobile-friendly

### JSFiddle (for Web Development)
**Website:** [jsfiddle.net](https://jsfiddle.net)
- Test HTML, CSS, JavaScript instantly
- Live preview
- Save and share your code

---

## 💾 Offline Learning Tips

### Save Lessons for Offline Reading
1. Open this repository in GitHub Mobile app
2. Star the repository ⭐
3. Open any lesson file
4. Tap the **Share** button
5. Choose "Save to Files" or "Download"

### Download Code Examples
- Copy code from lessons
- Paste into your mobile editor
- Practice offline anytime

---

## ⚡ Recommended Setup for Each Language

### For C Programming:
**Option 1:** Termux (Android)
```bash
pkg install clang
nano hello.c
clang hello.c -o hello
./hello
```

**Option 2:** OnlineGDB (any device)

---

### For C# and .NET:
**Option 1:** .NET MAUI on Termux (advanced)
**Option 2:** Replit (easier for beginners)

---

### For JavaScript:
**Option 1:** Spck Editor (web projects)
**Option 2:** Termux with Node.js
```bash
pkg install nodejs
node script.js
```

---

### For Assembly:
**Option 1:** Termux with NASM
```bash
pkg install nasm binutils
nasm -f elf64 program.asm
ld program.o -o program
./program
```

**Option 2:** Online x86 Assembly Simulator

---

### For Web Development (HTML/CSS/JS):
**Option 1:** Spck Editor (best experience)
**Option 2:** Acode + browser preview
**Option 3:** JSFiddle online

---

## 📊 Comparison Table

| Tool | Platform | Offline? | Best For | Free? |
|------|----------|----------|----------|-------|
| Termux | Android | ✅ Yes | C, Assembly, Python, JS | ✅ |
| Spck | Android/iOS | Partial | Web development | ✅ |
| Acode | Android | ✅ Yes | General editing | ✅ |
| Dcoder | Android/iOS | ❌ No | Quick testing | Free tier |
| Replit | Any (browser) | ❌ No | All languages | Free tier |
| OnlineGDB | Any (browser) | ❌ No | C/C++/Assembly | ✅ |

---

## 💡 Pro Tips

### Save Your Data Plan:
1. Download lessons when on WiFi
2. Use Termux for offline coding
3. Save code examples locally

### Keyboard Shortcuts:
- Most editors support external Bluetooth keyboards
- Makes coding much faster!

### Power Management:
- Mobile compilers can drain battery
- Keep your phone cool during intensive compilation

### Storage:
- Code files are tiny (usually < 1KB)
- You can store thousands of lessons and programs

---

## 🆘 Troubleshooting

### Termux not working?
- Download from F-Droid, not Google Play (better support)
- Grant storage permissions
- Update packages: `pkg update && pkg upgrade`

### Code won't run?
- Check syntax errors carefully
- Verify you have the right compiler installed
- Try online compiler to test if it's a setup issue

### Screen too small?
- Use landscape mode
- Adjust font size in editor settings
- Consider split-screen with lesson + editor

---

## 🎯 Getting Started Checklist

- [ ] Install GitHub Mobile app
- [ ] Choose and install a code editor
- [ ] If using Termux, install compilers
- [ ] Download your first lesson
- [ ] Write your first "Hello World"
- [ ] Save your work
- [ ] Join our community discussions

---

## 🌍 Low-Bandwidth Tips

**Saving data while learning:**
- GitHub Mobile has offline mode
- Download lessons in batches
- Use text-only mode when possible
- Most code examples are tiny in size

**Recommended data usage:**
- This entire repository: ~5-10 MB
- Single lesson: ~5-50 KB
- Code examples: < 1 KB each

---

## 🤝 Community Support

**Need help with mobile setup?**
- Open a [discussion](https://github.com/afrowaveltd/afrowave-learning/discussions)
- Tag your question with `mobile-setup`
- Share which device and tools you're using

---

## 📚 Next Steps

1. Pick your tool from the list above
2. Install it on your device
3. Go to [`lessons/`](../lessons/) folder
4. Choose a programming language
5. Start with lesson 01
6. Code along on your phone!

---

**Made with 💙 by the Afrowave Community**

> "The best time to start learning was yesterday. The second best time is now — even if you only have a phone!"