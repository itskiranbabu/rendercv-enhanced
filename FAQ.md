# ❓ Frequently Asked Questions (FAQ)

**Quick answers to common questions about RenderCV Enhanced**

*Curated by [itskiranbabu](https://github.com/itskiranbabu) | Powered by KeyRun AI*

---

## 📋 Table of Contents

1. [General Questions](#general-questions)
2. [Installation & Setup](#installation--setup)
3. [Usage & Features](#usage--features)
4. [Customization](#customization)
5. [Troubleshooting](#troubleshooting)
6. [AI Learning Resources](#ai-learning-resources)
7. [Contributing](#contributing)
8. [Support](#support)

---

## General Questions

### What is RenderCV Enhanced?

**RenderCV Enhanced** is an improved version of the popular RenderCV tool that generates professional CVs/resumes from YAML files. It includes:
- Comprehensive documentation
- 50+ AI/ML learning resources
- Best practices guide
- Career resources
- Community support
- Professional branding

### Is RenderCV Enhanced free?

**Yes!** RenderCV Enhanced is completely free and open-source under the MIT License. You can:
- Use it for personal or commercial purposes
- Modify it as needed
- Distribute it freely
- Contribute improvements

### How is this different from original RenderCV?

**Enhanced Features:**
- ✅ 3x more comprehensive documentation
- ✅ 50+ curated AI/ML learning resources
- ✅ Best practices guide for CV writing
- ✅ Career resources (job prep, interviews, certifications)
- ✅ Community integration (WhatsApp channels)
- ✅ Professional branding
- ✅ Troubleshooting guides
- ✅ FAQ section

**Core Features** (from original):
- YAML-based CV creation
- Multiple professional themes
- Perfect typography
- ATS-optimized output
- Multi-language support

### Who should use RenderCV Enhanced?

**Perfect for:**
- Software engineers
- Data scientists
- AI/ML professionals
- Students and recent graduates
- Career switchers
- Academic researchers
- Anyone needing a professional CV

### Do I need programming knowledge?

**Minimal programming needed:**
- Basic text editing (YAML format)
- Command-line basics (optional)
- Python installation (one-time setup)

**No need for:**
- Advanced programming
- LaTeX knowledge
- Design skills
- Typography expertise

---

## Installation & Setup

### What are the system requirements?

**Minimum Requirements:**
- **Python**: 3.12 or higher
- **pip**: Python package manager
- **Operating System**: Windows, macOS, or Linux
- **Disk Space**: ~100MB
- **RAM**: 512MB minimum

**Recommended:**
- Python 3.12+
- 1GB RAM
- Text editor (VS Code recommended)

### How do I install RenderCV Enhanced?

**Method 1: pip (Recommended)**
```bash
pip install "rendercv[full]"
```

**Method 2: From Source**
```bash
git clone https://github.com/itskiranbabu/rendercv-enhanced.git
cd rendercv-enhanced
pip install -e ".[full]"
```

**Method 3: Docker**
```bash
docker pull rendercv/rendercv:latest
```

See [Installation Guide](DOCUMENTATION.md#installation) for details.

### Do I need LaTeX installed?

**No!** RenderCV uses Typst (included in the `[full]` installation), which is simpler and faster than LaTeX.

If you install the minimal version (`pip install rendercv`), you'll need to install Typst separately.

### How do I verify installation?

```bash
# Check version
rendercv --version

# Get help
rendercv --help

# Test with example
rendercv new "Test User"
rendercv render Test_User_CV.yaml
```

### Can I use it offline?

**Yes!** Once installed, RenderCV works completely offline. No internet connection needed for:
- Creating CVs
- Rendering PDFs
- Customizing themes

Internet only needed for:
- Initial installation
- Downloading fonts (optional)
- Accessing online documentation

---

## Usage & Features

### How do I create my first CV?

**Quick Start (5 minutes):**

1. **Create template**
   ```bash
   rendercv new "Your Name"
   ```

2. **Edit YAML file**
   Open `Your_Name_CV.yaml` in text editor

3. **Generate PDF**
   ```bash
   rendercv render Your_Name_CV.yaml
   ```

See [Quick Start Guide](DOCUMENTATION.md#getting-started) for details.

### What file formats are supported?

**Input:**
- YAML (.yaml, .yml)

**Output:**
- PDF (default, recommended)
- Typst (.typ) - source file
- Markdown (.md) - text version

### How do I change themes?

**In your YAML file:**
```yaml
design:
  theme: moderncv  # Change to desired theme
```

**Available themes:**
- `classic` - Traditional, professional
- `moderncv` - Modern, colorful
- `sb2nov` - Minimalist
- `engineeringresumes` - Tech-focused
- `engineeringclassic` - Engineering traditional

Then regenerate:
```bash
rendercv render Your_CV.yaml
```

### Can I create custom themes?

**Yes!** You can create custom themes by:
1. Copying an existing theme
2. Modifying colors, fonts, spacing
3. Creating custom Typst templates

See [Theme Customization Guide](THEME_GUIDE.md) (coming soon).

### How do I add a photo?

**Photos are NOT recommended** for most CVs because:
- ATS systems may reject them
- Can introduce bias
- Not standard in US/UK

**If required:**
Custom theme needed. Contact community for help.

### Can I have multiple pages?

**Yes!** Content automatically flows to multiple pages. No manual page breaks needed.

**Recommended length:**
- 1 page: 0-5 years experience
- 2 pages: 5+ years experience
- 2+ pages: Academic CVs

### How do I add links?

**In YAML:**
```yaml
cv:
  website: https://yourwebsite.com
  
  social_networks:
    - network: LinkedIn
      username: yourprofile
    - network: GitHub
      username: yourprofile
```

Links are automatically formatted and clickable in PDF.

### Is it ATS-friendly?

**Yes!** All themes are optimized for Applicant Tracking Systems (ATS):
- Simple, clean formatting
- Standard section names
- No images or graphics
- Standard fonts
- PDF format
- Proper text extraction

See [ATS Optimization Guide](BEST_PRACTICES.md#ats-optimization).

---

## Customization

### How do I change colors?

**In your YAML file:**
```yaml
design:
  colors:
    name: rgb(0, 79, 144)        # Your name
    section_titles: rgb(0, 79, 144)  # Headers
    links: rgb(0, 79, 144)       # Hyperlinks
    body: rgb(0, 0, 0)           # Body text
```

**Color formats:**
- RGB: `rgb(255, 0, 0)`
- Hex: `#FF0000`
- Named: `red`, `blue`, `green`

### How do I change fonts?

**In your YAML file:**
```yaml
design:
  typography:
    font_family: Source Sans 3  # Font name
    font_size: 10pt             # Base size
```

**Available fonts:**
- Source Sans 3 (default)
- Latin Modern Roman
- Roboto
- Open Sans
- Lato
- Any system font

### How do I adjust spacing?

**In your YAML file:**
```yaml
design:
  typography:
    line_spacing: 0.6em  # Space between lines
  
  page:
    top_margin: 0.7in
    bottom_margin: 0.7in
    left_margin: 0.7in
    right_margin: 0.7in
```

### Can I change page size?

**Yes!**
```yaml
design:
  page:
    size: us-letter  # or a4
```

**Options:**
- `us-letter` - 8.5" × 11" (US standard)
- `a4` - 210mm × 297mm (International)

### How do I customize sections?

**Add/remove sections in YAML:**
```yaml
sections:
  summary: [...]
  experience: [...]
  education: [...]
  skills: [...]
  projects: [...]      # Optional
  certifications: [...] # Optional
  publications: [...]   # Optional
```

Order in YAML = order in CV.

---

## Troubleshooting

### "rendercv: command not found"

**Solution:**
```bash
# Ensure pip install location is in PATH
python -m pip install --user "rendercv[full]"

# Or use python -m
python -m rendercv render CV.yaml
```

### PDF not generating

**Solution:**
```bash
# Install full version with PDF support
pip install "rendercv[full]"

# Or install Typst separately
# See: https://github.com/typst/typst
```

### YAML validation errors

**Common issues:**
- Incorrect indentation (use 2 spaces)
- Missing colons after keys
- Incorrect date format (use YYYY-MM)
- Missing quotes for special characters

**Solution:**
- Use VS Code with YAML extension
- Validate online: https://www.yamllint.com/
- Check example files

### Fonts not working

**Solution:**
```bash
# Install rendercv-fonts package
pip install rendercv-fonts

# Or use system fonts
design:
  typography:
    font_family: Arial  # System font
```

### PDF looks different from expected

**Check:**
- Theme selection
- Color settings
- Font settings
- Margin settings
- Content length

**Solution:**
- Compare with example files
- Check YAML syntax
- Try different theme
- Ask community for help

### How do I update RenderCV?

```bash
# Check current version
rendercv --version

# Update to latest
pip install --upgrade "rendercv[full]"

# Verify update
rendercv --version
```

---

## AI Learning Resources

### Where are the AI learning resources?

**In this repository:**
- [README.md - AI Resources Section](README.md#-ai-learning-resources)
- [AI_RESOURCES.md - Complete Guide](AI_RESOURCES.md)

**Topics covered:**
- Beginner courses (Fast.ai, Coursera, Google)
- Books (Deep Learning for Coders, Hands-On ML)
- YouTube channels (3Blue1Brown, StatQuest)
- Intermediate resources (Stanford CS229, MIT)
- Advanced topics (NLP, CV, RL)
- Tools (TensorFlow, PyTorch, Scikit-learn)
- Career resources (LeetCode, Kaggle, certifications)

### Are the AI resources free?

**Most are free!**
- ✅ Fast.ai courses - Free
- ✅ Google ML Crash Course - Free
- ✅ YouTube channels - Free
- ✅ Many books available online - Free
- ✅ Kaggle - Free
- ✅ GitHub - Free

**Some paid options:**
- Coursera certificates - $49-79
- DataCamp subscription - $25/month
- Certifications - $100-300

### How do I start learning AI?

**Recommended path:**

**Month 1-3: Foundations**
1. Learn Python (if needed)
2. Take Fast.ai course
3. Practice on Kaggle

**Month 4-6: Core ML**
4. Andrew Ng's ML course
5. Read "Hands-On ML" book
6. Build first project

**Month 7-9: Deep Learning**
7. Deep Learning Specialization
8. Choose specialization (NLP/CV/RL)
9. Build portfolio projects

**Month 10-12: Career**
10. LeetCode practice
11. Get certification
12. Apply for jobs

See [AI Learning Roadmap](AI_RESOURCES.md#learning-roadmap).

### Which AI certification should I get?

**Popular certifications:**

**For Cloud:**
- Google Cloud Professional ML Engineer
- AWS Certified Machine Learning
- Microsoft Azure AI Engineer

**For ML:**
- TensorFlow Developer Certificate
- Deep Learning Specialization

**Choose based on:**
- Your career goals
- Company requirements
- Budget
- Time available

See [Certifications Guide](AI_RESOURCES.md#-certifications).

---

## Contributing

### How can I contribute?

**Ways to contribute:**
1. **Report bugs** - Found an issue? [Open an issue](https://github.com/itskiranbabu/rendercv-enhanced/issues)
2. **Suggest features** - Have an idea? [Create feature request](https://github.com/itskiranbabu/rendercv-enhanced/issues/new)
3. **Improve docs** - Fix typos, add examples
4. **Add AI resources** - Share learning resources
5. **Create themes** - Design new CV themes
6. **Write code** - Fix bugs, add features

See [Contributing Guide](CONTRIBUTING.md) for details.

### Do I need to be an expert?

**No!** All contributions welcome:
- Beginners can fix typos, improve docs
- Intermediate can add examples, resources
- Advanced can create themes, add features

**Good first issues** labeled for beginners.

### How do I submit a pull request?

**Steps:**
1. Fork the repository
2. Create a branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Commit (`git commit -m 'Add amazing feature'`)
5. Push (`git push origin feature/amazing-feature`)
6. Open Pull Request

See [Contributing Guide](CONTRIBUTING.md#pull-request-process).

---

## Support

### Where can I get help?

**Documentation:**
- [Complete Documentation](DOCUMENTATION.md)
- [Best Practices Guide](BEST_PRACTICES.md)
- [AI Resources](AI_RESOURCES.md)
- [This FAQ](FAQ.md)

**Community:**
- [WhatsApp Channel](https://whatsapp.com/channel/0029VbCCj7FGJP8EeBLXzD1C) - Daily insights
- [WhatsApp Group](https://chat.whatsapp.com/IfIKh4bVhCc1qjPEOFKQeh) - Discussions
- [GitHub Discussions](https://github.com/itskiranbabu/rendercv-enhanced/discussions) - Q&A
- [GitHub Issues](https://github.com/itskiranbabu/rendercv-enhanced/issues) - Bug reports

**Contact:**
- Email: itskeyrun.ai@gmail.com
- LinkedIn: [itskiranbabu](https://linkedin.com/in/itskiranbabu)
- GitHub: [@itskiranbabu](https://github.com/itskiranbabu)

### How do I report a bug?

1. **Check if already reported** - [Search issues](https://github.com/itskiranbabu/rendercv-enhanced/issues)
2. **Gather information** - Error messages, steps to reproduce
3. **Create issue** - [New bug report](https://github.com/itskiranbabu/rendercv-enhanced/issues/new?template=bug_report.md)
4. **Provide details** - OS, Python version, RenderCV version

### How do I request a feature?

1. **Check if already requested** - [Search issues](https://github.com/itskiranbabu/rendercv-enhanced/issues)
2. **Describe feature** - What problem does it solve?
3. **Create request** - [New feature request](https://github.com/itskiranbabu/rendercv-enhanced/issues/new?template=feature_request.md)
4. **Provide examples** - How would it work?

### Is there a community?

**Yes! Join us:**

**WhatsApp Channel** (Daily Content)
- Link: https://whatsapp.com/channel/0029VbCCj7FGJP8EeBLXzD1C
- Daily AI, Tech & Agile insights
- Career tips and resources
- 500+ members

**WhatsApp Group** (Discussions)
- Link: https://chat.whatsapp.com/IfIKh4bVhCc1qjPEOFKQeh
- Interactive discussions
- Q&A and support
- Networking

**GitHub Discussions**
- Link: https://github.com/itskiranbabu/rendercv-enhanced/discussions
- Technical discussions
- Feature requests
- Community support

---

## Additional Questions

### Can I use this for commercial purposes?

**Yes!** MIT License allows:
- Personal use
- Commercial use
- Modification
- Distribution

### Can I sell CVs created with RenderCV?

**Yes!** You can:
- Offer CV writing services
- Charge for customization
- Use in your business

### How do I cite RenderCV Enhanced?

**Citation:**
```
RenderCV Enhanced by itskiranbabu
https://github.com/itskiranbabu/rendercv-enhanced
Based on RenderCV by Sina Atalay
```

### Is my data private?

**Yes!** RenderCV:
- Runs locally on your computer
- No data sent to servers
- No tracking or analytics
- Your CV stays private

### Can I use it for academic CVs?

**Yes!** Perfect for academic CVs:
- Publications section
- Research interests
- Teaching experience
- Grants and awards
- No page limit

### How often is it updated?

**Regular updates:**
- Bug fixes: As needed
- Minor releases: Quarterly
- Major releases: Annually

**Stay updated:**
- Watch repository
- Join WhatsApp channel
- Follow on GitHub

### Can I translate it to my language?

**Yes!** RenderCV supports any language:
```yaml
locale:
  language: spanish  # or any language
  month_abbreviations:
    - Ene
    - Feb
    - Mar
    # ...
```

### Where can I see examples?

**Examples available:**
- [examples/ directory](examples/)
- [README.md examples](README.md#-examples)
- [BEST_PRACTICES.md examples](BEST_PRACTICES.md#examples)

---

## Still Have Questions?

**Can't find your answer?**

1. **Search documentation** - Use Ctrl+F to search
2. **Check GitHub issues** - Someone may have asked
3. **Ask community** - WhatsApp or GitHub Discussions
4. **Contact us** - itskeyrun.ai@gmail.com

**We're here to help!** 🚀

---

*Curated by [itskiranbabu](https://github.com/itskiranbabu) | Powered by KeyRun AI*
