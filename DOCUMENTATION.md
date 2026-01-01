# 📚 Complete Documentation - RenderCV Enhanced

**Comprehensive guide to using RenderCV Enhanced**

*Curated by [itskiranbabu](https://github.com/itskiranbabu) | Powered by KeyRun AI*

---

## Table of Contents

1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Getting Started](#getting-started)
4. [YAML Structure](#yaml-structure)
5. [Customization](#customization)
6. [Themes](#themes)
7. [Advanced Features](#advanced-features)
8. [Troubleshooting](#troubleshooting)
9. [Best Practices](#best-practices)
10. [FAQ](#faq)

---

## Introduction

### What is RenderCV?

RenderCV is a LaTeX-based CV/resume generator that takes your CV content in YAML format and produces a professionally formatted PDF with perfect typography.

### Why Use RenderCV?

**Traditional Problems:**
- Template wrestling in Word/LaTeX
- Broken layouts when editing
- Inconsistent spacing
- No version control
- Time-consuming updates

**RenderCV Solutions:**
- Version control friendly (plain text)
- Focus on content, not formatting
- Perfect typography automatically
- Easy updates
- Multiple themes
- ATS-optimized

### Key Features

✅ **YAML-Based** - Simple, readable format
✅ **Multiple Themes** - 5+ professional themes
✅ **JSON Schema** - Autocomplete in VS Code
✅ **Perfect Typography** - Pixel-perfect alignment
✅ **Multi-Language** - Any language supported
✅ **Fast** - Quick PDF generation
✅ **Open Source** - MIT License

---

## Installation

### System Requirements

- **Python**: 3.12 or higher
- **pip**: Python package manager
- **Operating System**: Windows, macOS, Linux

### Installation Methods

#### Method 1: pip (Recommended)

```bash
# Install with all features (includes PDF generation)
pip install "rendercv[full]"

# Verify installation
rendercv --version
```

#### Method 2: pip (Minimal)

```bash
# Install without PDF generation (generates Typst files only)
pip install rendercv

# You'll need to install Typst separately
# See: https://github.com/typst/typst
```

#### Method 3: From Source

```bash
# Clone repository
git clone https://github.com/itskiranbabu/rendercv-enhanced.git
cd rendercv-enhanced

# Install in development mode
pip install -e ".[full]"
```

#### Method 4: Docker

```bash
# Pull Docker image
docker pull rendercv/rendercv:latest

# Run RenderCV
docker run -v $(pwd):/data rendercv/rendercv render /data/CV.yaml
```

### Verify Installation

```bash
# Check version
rendercv --version

# Get help
rendercv --help

# Test with example
rendercv new "Test User"
rendercv render Test_User_CV.yaml
```

---

## Getting Started

### Quick Start (5 Minutes)

#### Step 1: Create Template

```bash
rendercv new "Your Name"
```

This creates `Your_Name_CV.yaml` with a complete template.

#### Step 2: Edit Your CV

Open `Your_Name_CV.yaml` in your favorite text editor (VS Code recommended).

**Basic Structure:**

```yaml
cv:
  name: Your Name
  location: City, Country
  email: your.email@example.com
  phone: "+1 234 567 8900"
  website: https://yourwebsite.com
  
  social_networks:
    - network: LinkedIn
      username: yourlinkedin
    - network: GitHub
      username: yourgithub
  
  sections:
    summary:
      - "Brief professional summary"
      - "Key achievements and skills"
    
    experience:
      - company: Company Name
        position: Your Position
        location: City, Country
        start_date: 2020-01
        end_date: present
        highlights:
          - "Achievement 1 with quantifiable results"
          - "Achievement 2 with impact"
    
    education:
      - institution: University Name
        area: Your Major
        degree: BS/MS/PhD
        start_date: 2016-09
        end_date: 2020-05
        location: City, Country
    
    skills:
      - label: Programming
        details: Python, JavaScript, Java
      - label: Frameworks
        details: React, Django, Flask

design:
  theme: classic
```

#### Step 3: Generate PDF

```bash
rendercv render Your_Name_CV.yaml
```

**Output Files:**
- `Your_Name_CV.pdf` - Your professional CV
- `Your_Name_CV.typ` - Typst source file
- `Your_Name_CV_MARKDOWN.md` - Markdown version

#### Step 4: Customize (Optional)

Change theme, colors, fonts, spacing, etc. See [Customization](#customization) section.

---

## YAML Structure

### Complete YAML Reference

```yaml
# ============================================
# CV CONTENT
# ============================================
cv:
  # Personal Information
  name: John Doe
  label: Software Engineer  # Optional job title
  location: San Francisco, CA
  email: john.doe@email.com
  phone: "+1 234 567 8900"
  website: https://johndoe.com
  
  # Social Networks
  social_networks:
    - network: LinkedIn
      username: johndoe
    - network: GitHub
      username: johndoe
    - network: Twitter
      username: johndoe
    - network: Instagram
      username: johndoe
  
  # CV Sections
  sections:
    # Summary Section
    summary:
      - "Experienced Software Engineer with 5+ years in full-stack development"
      - "Specialized in Python, React, and cloud technologies"
      - "Passionate about building scalable systems"
    
    # Experience Section
    experience:
      - company: Tech Corp
        position: Senior Software Engineer
        location: San Francisco, CA
        start_date: 2020-01
        end_date: present
        highlights:
          - "Led team of 5 engineers in microservices architecture"
          - "Reduced API response time by 40%"
          - "Implemented CI/CD pipeline"
      
      - company: StartupXYZ
        position: Software Engineer
        location: Remote
        start_date: 2018-06
        end_date: 2019-12
        highlights:
          - "Built RESTful APIs serving 1M+ requests daily"
          - "Developed React frontend with 95% test coverage"
    
    # Education Section
    education:
      - institution: University of California
        area: Computer Science
        degree: BS
        start_date: 2014-09
        end_date: 2018-05
        location: Berkeley, CA
        gpa: "3.8/4.0"
        highlights:
          - "Dean's List all semesters"
          - "President of Computer Science Club"
    
    # Skills Section
    skills:
      - label: Programming Languages
        details: Python, JavaScript, TypeScript, Go, Java
      - label: Frameworks & Libraries
        details: React, Node.js, Django, Flask, FastAPI
      - label: Cloud & DevOps
        details: AWS, GCP, Docker, Kubernetes, Terraform
      - label: Databases
        details: PostgreSQL, MongoDB, Redis, Elasticsearch
    
    # Projects Section (Optional)
    projects:
      - name: Open Source Project
        date: 2023
        highlights:
          - "Built CLI tool with 1000+ GitHub stars"
          - "Used by developers worldwide"
        url: https://github.com/username/project
    
    # Publications Section (Optional)
    publications:
      - title: "Paper Title"
        authors:
          - John Doe
          - Jane Smith
        date: 2023-05
        journal: Conference Name
        doi: 10.1234/example
    
    # Certifications Section (Optional)
    certifications:
      - name: AWS Certified Solutions Architect
        date: 2023-01
        url: https://aws.amazon.com/certification/
    
    # Awards Section (Optional)
    awards:
      - title: Best Paper Award
        date: 2023
        awarder: Conference Name
    
    # Languages Section (Optional)
    languages:
      - language: English
        fluency: Native
      - language: Spanish
        fluency: Professional

# ============================================
# DESIGN CONFIGURATION
# ============================================
design:
  # Theme Selection
  theme: classic  # Options: classic, moderncv, sb2nov, engineeringresumes, engineeringclassic
  
  # Page Settings
  page:
    size: us-letter  # Options: us-letter, a4
    top_margin: 0.7in
    bottom_margin: 0.7in
    left_margin: 0.7in
    right_margin: 0.7in
    show_footer: true
    show_top_note: true
  
  # Color Scheme
  colors:
    body: rgb(0, 0, 0)
    name: rgb(0, 79, 144)
    headline: rgb(0, 79, 144)
    connections: rgb(0, 79, 144)
    section_titles: rgb(0, 79, 144)
    links: rgb(0, 79, 144)
    footer: rgb(128, 128, 128)
    top_note: rgb(128, 128, 128)
  
  # Typography
  typography:
    line_spacing: 0.6em
    alignment: justified  # Options: justified, left, right, center
    date_and_location_column_alignment: right
    font_family: Source Sans 3
    font_size: 10pt
  
  # Header
  header:
    name_font_size: 24pt
    use_icons_for_connections: true
    separator_between_connections: " | "
  
  # Sections
  sections:
    section_title_font_size: 14pt
    entry_area_left_margin: 0.2in
    highlights_area_left_margin: 0.4in

# ============================================
# LOCALE CONFIGURATION
# ============================================
locale:
  language: english
  last_updated: Last updated in
  month: month
  months: months
  year: year
  years: years
  present: present
  month_abbreviations:
    - Jan
    - Feb
    - Mar
    - Apr
    - May
    - Jun
    - Jul
    - Aug
    - Sep
    - Oct
    - Nov
    - Dec
```

### Section Types

#### 1. Text Sections

Simple text entries (summary, objective):

```yaml
sections:
  summary:
    - "First paragraph"
    - "Second paragraph"
```

#### 2. Experience Entries

Work experience, internships:

```yaml
sections:
  experience:
    - company: Company Name
      position: Job Title
      location: City, Country
      start_date: 2020-01
      end_date: present  # or YYYY-MM
      highlights:
        - "Achievement 1"
        - "Achievement 2"
```

#### 3. Education Entries

Academic background:

```yaml
sections:
  education:
    - institution: University Name
      area: Major/Field
      degree: BS/MS/PhD
      start_date: 2016-09
      end_date: 2020-05
      location: City, Country
      gpa: "3.8/4.0"  # Optional
      highlights:
        - "Honor 1"
        - "Honor 2"
```

#### 4. Skill Entries

Technical and soft skills:

```yaml
sections:
  skills:
    - label: Category
      details: Skill1, Skill2, Skill3
```

#### 5. Project Entries

Personal or professional projects:

```yaml
sections:
  projects:
    - name: Project Name
      date: 2023
      highlights:
        - "Description 1"
        - "Description 2"
      url: https://project-url.com  # Optional
```

---

## Customization

### Changing Themes

```yaml
design:
  theme: moderncv  # Change to any available theme
```

**Available Themes:**
- `classic` - Traditional, professional
- `moderncv` - Modern, colorful
- `sb2nov` - Minimalist
- `engineeringresumes` - Tech-focused
- `engineeringclassic` - Engineering traditional

### Customizing Colors

```yaml
design:
  colors:
    name: rgb(0, 79, 144)        # Your name color
    section_titles: rgb(0, 79, 144)  # Section headers
    links: rgb(0, 79, 144)       # Hyperlinks
    body: rgb(0, 0, 0)           # Body text
```

**Color Formats:**
- RGB: `rgb(255, 0, 0)`
- Hex: `#FF0000`
- Named: `red`, `blue`, `green`

### Customizing Typography

```yaml
design:
  typography:
    font_family: Source Sans 3  # Font name
    font_size: 10pt             # Base font size
    line_spacing: 0.6em         # Space between lines
    alignment: justified        # Text alignment
```

**Available Fonts:**
- Source Sans 3
- Latin Modern Roman
- Roboto
- Open Sans
- Lato

### Page Layout

```yaml
design:
  page:
    size: us-letter  # or a4
    top_margin: 0.7in
    bottom_margin: 0.7in
    left_margin: 0.7in
    right_margin: 0.7in
```

### Header Customization

```yaml
design:
  header:
    name_font_size: 24pt
    use_icons_for_connections: true
    separator_between_connections: " | "
```

---

## Themes

### Theme Comparison

| Theme | Best For | Style | ATS-Friendly |
|-------|----------|-------|--------------|
| Classic | Academic, Traditional | Clean, Professional | ✅ Yes |
| Modern CV | Creative, Startups | Colorful, Modern | ✅ Yes |
| Sb2nov | Minimalist | Clean, Dense | ✅ Yes |
| Engineering Resumes | Tech, FAANG | Skills-focused | ✅ Yes |
| Engineering Classic | Engineering | Traditional Tech | ✅ Yes |

### Switching Themes

Simply change the theme in your YAML:

```yaml
design:
  theme: moderncv
```

Then regenerate:

```bash
rendercv render Your_CV.yaml
```

---

## Advanced Features

### Live Preview

Watch for file changes and auto-regenerate:

```bash
rendercv render CV.yaml --watch
```

### Custom Output Directory

```bash
rendercv render CV.yaml --output-folder ./output
```

### Generate Multiple Formats

```bash
# PDF only (default)
rendercv render CV.yaml

# Include Markdown
rendercv render CV.yaml --markdown

# Include Typst source
rendercv render CV.yaml --typst
```

### Batch Processing

```bash
# Render all YAML files
for cv in *.yaml; do
    rendercv render "$cv"
done
```

### VS Code Integration

1. Install YAML extension
2. Configure JSON Schema
3. Get autocomplete and validation

See [VS Code Setup Guide](https://docs.rendercv.com/user_guide/how_to/set_up_vs_code_for_rendercv)

---

## Troubleshooting

### Common Issues

#### Issue: "rendercv: command not found"

**Solution:**
```bash
# Ensure pip install location is in PATH
python -m pip install --user "rendercv[full]"

# Or use python -m
python -m rendercv render CV.yaml
```

#### Issue: PDF not generating

**Solution:**
```bash
# Install full version with PDF support
pip install "rendercv[full]"

# Or install Typst separately
# See: https://github.com/typst/typst
```

#### Issue: YAML validation errors

**Solution:**
- Check YAML syntax (indentation, colons, dashes)
- Use VS Code with YAML extension
- Validate online: https://www.yamllint.com/

#### Issue: Fonts not working

**Solution:**
```bash
# Install rendercv-fonts package
pip install rendercv-fonts

# Or use system fonts
design:
  typography:
    font_family: Arial  # System font
```

### Getting Help

1. **Check Documentation** - Read this guide thoroughly
2. **Search Issues** - [GitHub Issues](https://github.com/itskiranbabu/rendercv-enhanced/issues)
3. **Ask Community** - [GitHub Discussions](https://github.com/itskiranbabu/rendercv-enhanced/discussions)
4. **Report Bug** - [New Issue](https://github.com/itskiranbabu/rendercv-enhanced/issues/new)

---

## Best Practices

### Content Best Practices

✅ **Use action verbs** - Led, Developed, Implemented, Achieved
✅ **Quantify results** - Increased by 40%, Reduced by 60%
✅ **Be specific** - Technologies, team sizes, impact
✅ **Tailor to job** - Match keywords from job description
✅ **Keep concise** - 1-2 pages maximum
✅ **Proofread** - No typos or grammatical errors

### Formatting Best Practices

✅ **Consistent dates** - Use same format throughout
✅ **Reverse chronological** - Most recent first
✅ **Clear hierarchy** - Section > Company > Position > Achievements
✅ **Bullet points** - For achievements and responsibilities
✅ **White space** - Don't overcrowd

### ATS Optimization

✅ **Standard sections** - Experience, Education, Skills
✅ **Keywords** - From job description
✅ **Simple format** - RenderCV handles this
✅ **PDF format** - RenderCV default
✅ **Standard fonts** - Avoid fancy fonts

---

## FAQ

### General Questions

**Q: Is RenderCV free?**
A: Yes, completely free and open-source (MIT License).

**Q: Do I need LaTeX knowledge?**
A: No, RenderCV uses Typst (simpler than LaTeX).

**Q: Can I use custom fonts?**
A: Yes, any system font or install rendercv-fonts package.

**Q: Is it ATS-friendly?**
A: Yes, all themes are optimized for ATS.

**Q: Can I create custom themes?**
A: Yes, see Custom Theme Guide.

### Technical Questions

**Q: What Python version is required?**
A: Python 3.12 or higher.

**Q: Can I use it offline?**
A: Yes, once installed, works completely offline.

**Q: How do I update RenderCV?**
A: `pip install --upgrade "rendercv[full]"`

**Q: Can I contribute?**
A: Yes! See [Contributing Guide](CONTRIBUTING.md).

### Usage Questions

**Q: How do I add a photo?**
A: Photos are not recommended for ATS. If needed, use custom theme.

**Q: Can I have multiple pages?**
A: Yes, content automatically flows to multiple pages.

**Q: How do I change page size?**
A: Set `design.page.size` to `us-letter` or `a4`.

**Q: Can I export to Word?**
A: No, but you can export to Markdown and convert.

---

## Additional Resources

### Official Resources

- **Original RenderCV** - [github.com/rendercv/rendercv](https://github.com/rendercv/rendercv)
- **Documentation** - [docs.rendercv.com](https://docs.rendercv.com)
- **Typst** - [typst.app](https://typst.app)

### Community

- **WhatsApp Channel** - [Join Channel](https://whatsapp.com/channel/0029VbCCj7FGJP8EeBLXzD1C)
- **WhatsApp Group** - [Join Group](https://chat.whatsapp.com/IfIKh4bVhCc1qjPEOFKQeh)
- **GitHub Discussions** - [Discussions](https://github.com/itskiranbabu/rendercv-enhanced/discussions)

### Learning Resources

- **AI Learning Resources** - See [README](README.md#-ai-learning-resources)
- **Career Resources** - Resume tips, interview prep
- **Best Practices** - Industry standards

---

**Need more help? [Open an issue](https://github.com/itskiranbabu/rendercv-enhanced/issues) or [join our community](https://whatsapp.com/channel/0029VbCCj7FGJP8EeBLXzD1C)!**

---

*Curated by [itskiranbabu](https://github.com/itskiranbabu) | Powered by KeyRun AI*
