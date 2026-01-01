<div align="center">

# 🚀 RenderCV Enhanced

*Professional CV/Resume Generator with AI Learning Resources*

[![GitHub Stars](https://img.shields.io/github/stars/itskiranbabu/rendercv-enhanced?style=social)](https://github.com/itskiranbabu/rendercv-enhanced/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/itskiranbabu/rendercv-enhanced?style=social)](https://github.com/itskiranbabu/rendercv-enhanced/network/members)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.12+](https://img.shields.io/badge/python-3.12+-blue.svg)](https://www.python.org/downloads/)
[![Documentation](https://img.shields.io/badge/docs-enhanced-brightgreen.svg)](https://github.com/itskiranbabu/rendercv-enhanced/blob/main/DOCUMENTATION.md)

**Write your CV in YAML, get a PDF with perfect typography. No template wrestling. No broken layouts.**

*Enhanced with comprehensive documentation, AI learning resources, and professional branding*

[Features](#-features) • [Quick Start](#-quick-start) • [Documentation](#-documentation) • [AI Resources](#-ai-learning-resources) • [Examples](#-examples) • [Contributing](#-contributing)

---

**Curated by [itskiranbabu](https://github.com/itskiranbabu) | Powered by KeyRun AI**

</div>

---

## 📋 Table of Contents

- [What is RenderCV Enhanced?](#-what-is-rendercv-enhanced)
- [Why RenderCV Enhanced?](#-why-rendercv-enhanced)
- [Features](#-features)
- [Quick Start](#-quick-start)
- [Installation](#-installation)
- [Usage](#-usage)
- [Themes](#-themes)
- [Documentation](#-documentation)
- [AI Learning Resources](#-ai-learning-resources)
- [Examples](#-examples)
- [Best Practices](#-best-practices)
- [Contributing](#-contributing)
- [Community](#-community)
- [License](#-license)
- [Acknowledgments](#-acknowledgments)

---

## 🎯 What is RenderCV Enhanced?

**RenderCV Enhanced** is a powerful, enhanced version of the popular RenderCV tool that transforms your CV/resume from YAML format into beautifully formatted PDFs with perfect typography.

### Key Enhancements:

✅ **Comprehensive Documentation** - Step-by-step guides for all skill levels
✅ **AI Learning Resources** - Curated collection of AI/ML learning materials
✅ **Professional Templates** - 5+ professionally designed themes
✅ **Best Practices Guide** - Industry-standard CV writing tips
✅ **Career Resources** - Job search strategies and interview prep
✅ **Community Support** - Active community and regular updates

---

## 💡 Why RenderCV Enhanced?

### Traditional CV Tools Problems:

❌ Template wrestling with Word/LaTeX
❌ Broken layouts when editing
❌ Inconsistent spacing and formatting
❌ No version control
❌ Time-consuming updates

### RenderCV Enhanced Solutions:

✅ **Version Control** - Your CV is just text (YAML)
✅ **Focus on Content** - No formatting headaches
✅ **Perfect Typography** - Pixel-perfect alignment every time
✅ **Easy Updates** - Change once, perfect everywhere
✅ **Professional Output** - Industry-standard PDFs
✅ **Multiple Themes** - Switch themes instantly
✅ **JSON Schema** - Autocomplete and validation in VS Code

---

## ✨ Features

### Core Features

🎨 **Multiple Professional Themes**
- Classic
- Modern CV
- Engineering Resumes
- Sb2nov
- Engineering Classic
- Custom themes support

📝 **YAML-Based**
- Simple, readable format
- Version control friendly
- Easy to maintain
- Supports all CV sections

🔍 **JSON Schema Support**
- Autocomplete in VS Code
- Inline documentation
- Real-time validation
- Error prevention

🎯 **Perfect Typography**
- Pixel-perfect alignment
- Consistent spacing
- Professional fonts
- Optimized for ATS

🌍 **Multi-Language Support**
- Any language supported
- Customizable locale
- Date format options
- Month abbreviations

⚡ **Fast & Efficient**
- Quick PDF generation
- Live preview support
- Batch processing
- Command-line interface

### Enhanced Features

📚 **Comprehensive Documentation**
- Beginner-friendly guides
- Advanced customization
- Troubleshooting tips
- Video tutorials

🤖 **AI Learning Resources**
- Curated AI/ML courses
- Research papers
- Tutorial collections
- Career guidance

💼 **Career Resources**
- Resume writing tips
- Interview preparation
- Job search strategies
- Salary negotiation

🎓 **Educational Content**
- Best practices guide
- Industry standards
- ATS optimization
- Design principles

---

## 🚀 Quick Start

### 1. Install RenderCV

```bash
pip install "rendercv[full]"
```

### 2. Create Your CV

```bash
rendercv new "Your Name"
```

This creates `Your_Name_CV.yaml` with a template.

### 3. Edit Your CV

Open `Your_Name_CV.yaml` in your favorite editor (VS Code recommended) and fill in your information.

### 4. Generate PDF

```bash
rendercv render Your_Name_CV.yaml
```

Your professional PDF is ready! 🎉

---

## 📦 Installation

### Requirements

- Python 3.12 or higher
- pip (Python package manager)

### Installation Methods

#### Method 1: pip (Recommended)

```bash
# Install with all features
pip install "rendercv[full]"

# Install minimal version (no PDF generation)
pip install rendercv
```

#### Method 2: From Source

```bash
# Clone this repository
git clone https://github.com/itskiranbabu/rendercv-enhanced.git
cd rendercv-enhanced

# Install dependencies
pip install -e ".[full]"
```

#### Method 3: Docker

```bash
# Pull Docker image
docker pull rendercv/rendercv:latest

# Run RenderCV
docker run -v $(pwd):/data rendercv/rendercv render /data/Your_CV.yaml
```

### Verify Installation

```bash
rendercv --version
```

---

## 📖 Usage

### Basic Commands

#### Create New CV

```bash
rendercv new "John Doe"
```

Creates `John_Doe_CV.yaml` with template structure.

#### Render CV to PDF

```bash
rendercv render John_Doe_CV.yaml
```

Generates:
- `John_Doe_CV.pdf` - Your professional CV
- `John_Doe_CV.typ` - Typst source file
- `John_Doe_CV_MARKDOWN.md` - Markdown version

#### Live Preview

```bash
rendercv render John_Doe_CV.yaml --watch
```

Automatically regenerates PDF when you save changes.

#### Custom Output Directory

```bash
rendercv render John_Doe_CV.yaml --output-folder ./output
```

#### Specific Theme

```bash
rendercv render John_Doe_CV.yaml --theme moderncv
```

### Advanced Usage

#### Batch Processing

```bash
# Render multiple CVs
for cv in *.yaml; do
    rendercv render "$cv"
done
```

#### Custom Configuration

```bash
# Use custom config file
rendercv render CV.yaml --config custom_config.yaml
```

#### Export to Multiple Formats

```bash
# Generate PDF, Markdown, and Typst
rendercv render CV.yaml --pdf --markdown --typst
```

---

## 🎨 Themes

RenderCV Enhanced includes 5 professional themes:

### 1. Classic Theme

**Best For:** Academic positions, research roles, traditional industries

**Features:**
- Clean, professional layout
- Emphasis on content
- Traditional typography
- ATS-friendly

**Preview:** [View Example](examples/John_Doe_ClassicTheme_CV.pdf)

### 2. Modern CV Theme

**Best For:** Creative roles, startups, modern companies

**Features:**
- Contemporary design
- Color accents
- Modern typography
- Visual hierarchy

**Preview:** [View Example](examples/John_Doe_ModerncvTheme_CV.pdf)

### 3. Engineering Resumes Theme

**Best For:** Software engineers, tech roles, FAANG applications

**Features:**
- Optimized for tech industry
- Skills-focused layout
- Project highlights
- GitHub integration

**Preview:** [View Example](examples/John_Doe_EngineeringresumesTheme_CV.pdf)

### 4. Sb2nov Theme

**Best For:** Minimalist preference, clean design lovers

**Features:**
- Minimalist design
- Maximum content density
- Clean typography
- Efficient use of space

**Preview:** [View Example](examples/John_Doe_Sb2novTheme_CV.pdf)

### 5. Engineering Classic Theme

**Best For:** Engineering roles, technical positions

**Features:**
- Technical focus
- Clear sections
- Professional appearance
- Industry-standard

**Preview:** [View Example](examples/John_Doe_EngineeringclassicTheme_CV.pdf)

### Custom Themes

Create your own theme! See [Custom Theme Guide](CUSTOM_THEMES.md)

---

## 📚 Documentation

### Complete Documentation

- **[User Guide](DOCUMENTATION.md)** - Complete usage guide
- **[YAML Structure](YAML_GUIDE.md)** - YAML format reference
- **[Theme Customization](THEME_GUIDE.md)** - Create custom themes
- **[Best Practices](BEST_PRACTICES.md)** - CV writing tips
- **[Troubleshooting](TROUBLESHOOTING.md)** - Common issues & solutions
- **[API Reference](API_REFERENCE.md)** - Developer documentation

### Quick References

- **[Cheat Sheet](CHEAT_SHEET.md)** - Quick command reference
- **[FAQ](FAQ.md)** - Frequently asked questions
- **[Examples](examples/)** - Sample CVs and templates

---

## 🤖 AI Learning Resources

### Why AI Learning Resources?

As technology evolves, staying updated with AI/ML is crucial for career growth. This section provides curated resources for learning AI from scratch to advanced levels.

### 📚 Beginner Resources

#### Online Courses

1. **[Fast.ai - Practical Deep Learning](https://course.fast.ai/)**
   - Free, practical approach
   - No prerequisites required
   - Hands-on projects
   - Duration: 9 lessons (~90 min each)

2. **[DeepLearning.AI - AI For Everyone](https://www.coursera.org/learn/ai-for-everyone)**
   - Non-technical introduction
   - Business applications
   - AI strategy
   - Duration: 4 weeks

3. **[Google's Machine Learning Crash Course](https://developers.google.com/machine-learning/crash-course)**
   - Free from Google
   - TensorFlow tutorials
   - Interactive exercises
   - Duration: 15 hours

4. **[Andrew Ng's Machine Learning](https://www.coursera.org/learn/machine-learning)**
   - Classic ML course
   - Mathematical foundations
   - Practical assignments
   - Duration: 11 weeks

#### Books

1. **"Deep Learning for Coders" by Jeremy Howard**
   - Practical approach
   - Code-first learning
   - Free online: [book.fast.ai](https://book.fast.ai)

2. **"Hands-On Machine Learning" by Aurélien Géron**
   - Comprehensive guide
   - Scikit-Learn & TensorFlow
   - Practical examples

3. **"Python Machine Learning" by Sebastian Raschka**
   - Python-focused
   - Step-by-step tutorials
   - Real-world applications

#### YouTube Channels

1. **[3Blue1Brown](https://www.youtube.com/c/3blue1brown)** - Visual math explanations
2. **[StatQuest](https://www.youtube.com/c/joshstarmer)** - ML concepts simplified
3. **[Sentdex](https://www.youtube.com/c/sentdex)** - Python & ML tutorials
4. **[Andrej Karpathy](https://www.youtube.com/@AndrejKarpathy)** - Deep learning lectures

### 🚀 Intermediate Resources

#### Advanced Courses

1. **[Stanford CS229 - Machine Learning](https://cs229.stanford.edu/)**
   - University-level course
   - Mathematical depth
   - Research-oriented

2. **[MIT 6.S191 - Deep Learning](http://introtodeeplearning.com/)**
   - Comprehensive DL course
   - Latest techniques
   - Guest lectures

3. **[Deep Learning Specialization](https://www.coursera.org/specializations/deep-learning)**
   - 5-course series
   - Neural networks
   - Practical projects

#### Research Papers

1. **[Papers With Code](https://paperswithcode.com/)** - Latest research with code
2. **[arXiv.org](https://arxiv.org/list/cs.AI/recent)** - AI research papers
3. **[Distill.pub](https://distill.pub/)** - Interactive ML research

#### Tools & Frameworks

1. **TensorFlow** - Google's ML framework
2. **PyTorch** - Facebook's DL framework
3. **Scikit-learn** - Classical ML library
4. **Keras** - High-level neural networks API
5. **Hugging Face** - NLP models & datasets

### 💼 Career Resources

#### Job Preparation

1. **[LeetCode](https://leetcode.com/)** - Coding interview prep
2. **[Kaggle](https://www.kaggle.com/)** - ML competitions & datasets
3. **[GitHub](https://github.com/)** - Portfolio projects

#### Interview Prep

1. **"Cracking the Coding Interview"** - Technical interviews
2. **"Machine Learning Interview Book"** - ML-specific questions
3. **[Interview Query](https://www.interviewquery.com/)** - Data science interviews

#### Certifications

1. **Google Cloud Professional ML Engineer**
2. **AWS Certified Machine Learning**
3. **TensorFlow Developer Certificate**
4. **Microsoft Azure AI Engineer**

### 🌟 Advanced Resources

#### Specialized Topics

1. **Natural Language Processing (NLP)**
   - [Hugging Face Course](https://huggingface.co/course)
   - [Stanford CS224N](http://web.stanford.edu/class/cs224n/)

2. **Computer Vision**
   - [Stanford CS231n](http://cs231n.stanford.edu/)
   - [PyImageSearch](https://www.pyimagesearch.com/)

3. **Reinforcement Learning**
   - [Spinning Up in Deep RL](https://spinningup.openai.com/)
   - [DeepMind x UCL RL Course](https://www.deepmind.com/learning-resources)

#### Communities

1. **[r/MachineLearning](https://www.reddit.com/r/MachineLearning/)** - Reddit community
2. **[AI Alignment Forum](https://www.alignmentforum.org/)** - AI safety discussions
3. **[Towards Data Science](https://towardsdatascience.com/)** - Medium publication
4. **[AI Innovators & Agile Leaders Hub](https://whatsapp.com/channel/0029VbCCj7FGJP8EeBLXzD1C)** - WhatsApp community

---

## 📂 Examples

### Sample CVs

All examples are available in the `examples/` directory:

1. **Academic CV** - For PhD students, researchers
2. **Software Engineer CV** - For tech roles
3. **Data Scientist CV** - For ML/AI positions
4. **Product Manager CV** - For PM roles
5. **Designer CV** - For creative positions

### YAML Templates

```yaml
cv:
  name: John Doe
  location: San Francisco, CA
  email: john.doe@email.com
  website: https://johndoe.com
  phone: "+1 234 567 8900"
  
  social_networks:
    - network: LinkedIn
      username: johndoe
    - network: GitHub
      username: johndoe
    - network: Twitter
      username: johndoe
  
  sections:
    summary:
      - "Experienced Software Engineer with 5+ years in full-stack development"
      - "Specialized in Python, React, and cloud technologies"
      - "Passionate about building scalable systems and mentoring teams"
    
    experience:
      - company: Tech Corp
        position: Senior Software Engineer
        location: San Francisco, CA
        start_date: 2020-01
        end_date: present
        highlights:
          - "Led team of 5 engineers in developing microservices architecture"
          - "Reduced API response time by 40% through optimization"
          - "Implemented CI/CD pipeline reducing deployment time by 60%"
      
      - company: StartupXYZ
        position: Software Engineer
        location: Remote
        start_date: 2018-06
        end_date: 2019-12
        highlights:
          - "Built RESTful APIs serving 1M+ requests daily"
          - "Developed React frontend with 95% test coverage"
          - "Mentored 3 junior developers"
    
    education:
      - institution: University of California
        area: Computer Science
        degree: BS
        start_date: 2014-09
        end_date: 2018-05
        location: Berkeley, CA
        highlights:
          - "GPA: 3.8/4.0"
          - "Dean's List all semesters"
          - "President of Computer Science Club"
    
    skills:
      - label: Programming
        details: Python, JavaScript, TypeScript, Go, Java
      - label: Frameworks
        details: React, Node.js, Django, Flask, FastAPI
      - label: Cloud
        details: AWS, GCP, Azure, Docker, Kubernetes
      - label: Databases
        details: PostgreSQL, MongoDB, Redis, Elasticsearch
      - label: Tools
        details: Git, CI/CD, Terraform, Jenkins

design:
  theme: classic
  page:
    size: us-letter
    top_margin: 0.7in
    bottom_margin: 0.7in
    left_margin: 0.7in
    right_margin: 0.7in
  colors:
    name: rgb(0, 79, 144)
    section_titles: rgb(0, 79, 144)
    links: rgb(0, 79, 144)
  typography:
    font_family: Source Sans 3
    line_spacing: 0.6em
```

---

## 💡 Best Practices

### CV Writing Tips

#### Content

✅ **DO:**
- Use action verbs (Led, Developed, Implemented)
- Quantify achievements (Increased by 40%, Reduced by 60%)
- Tailor to job description
- Keep it concise (1-2 pages)
- Highlight relevant skills
- Include keywords for ATS

❌ **DON'T:**
- Use personal pronouns (I, me, my)
- Include irrelevant information
- Use fancy fonts or colors (unless design role)
- Add photos (unless required)
- Include references (say "available upon request")

#### Structure

1. **Contact Information** - Name, email, phone, LinkedIn, GitHub
2. **Summary/Objective** - 2-3 sentences about you
3. **Experience** - Reverse chronological order
4. **Education** - Degree, institution, dates
5. **Skills** - Relevant technical skills
6. **Projects** (optional) - Personal/open-source projects
7. **Certifications** (optional) - Relevant certifications

#### Formatting

- **Consistent spacing** - Use RenderCV's automatic spacing
- **Clear hierarchy** - Section titles, job titles, dates
- **Bullet points** - For achievements and responsibilities
- **Dates** - Use consistent format (YYYY-MM or Month YYYY)
- **Length** - 1 page for <5 years experience, 2 pages for >5 years

### ATS Optimization

**Applicant Tracking Systems (ATS)** scan CVs before humans see them. Optimize for ATS:

✅ Use standard section names (Experience, Education, Skills)
✅ Include keywords from job description
✅ Use simple formatting (RenderCV handles this)
✅ Avoid tables, images, headers/footers
✅ Use standard fonts
✅ Save as PDF (RenderCV default)

### Industry-Specific Tips

#### Tech/Engineering
- Emphasize technical skills
- Include GitHub/portfolio links
- Highlight projects and contributions
- Mention technologies used

#### Academic/Research
- List publications
- Include research interests
- Mention grants and awards
- Add teaching experience

#### Business/Management
- Focus on leadership
- Quantify business impact
- Highlight team management
- Include strategic initiatives

---

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### Ways to Contribute

1. **Report Bugs** - Found an issue? [Open an issue](https://github.com/itskiranbabu/rendercv-enhanced/issues)
2. **Suggest Features** - Have an idea? [Create a feature request](https://github.com/itskiranbabu/rendercv-enhanced/issues/new)
3. **Improve Documentation** - Fix typos, add examples
4. **Add Resources** - Share AI learning resources
5. **Create Themes** - Design new CV themes
6. **Write Tutorials** - Help others learn

### Contribution Guidelines

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/amazing-feature`)
3. **Commit your changes** (`git commit -m 'Add amazing feature'`)
4. **Push to branch** (`git push origin feature/amazing-feature`)
5. **Open a Pull Request**

### Code of Conduct

- Be respectful and inclusive
- Provide constructive feedback
- Help others learn
- Follow coding standards
- Test your changes

---

## 👥 Community

### Join Our Community

📱 **WhatsApp Channel** - Daily AI & Tech insights
🔗 [Join Channel](https://whatsapp.com/channel/0029VbCCj7FGJP8EeBLXzD1C)

💬 **WhatsApp Group** - Interactive discussions
🔗 [Join Group](https://chat.whatsapp.com/IfIKh4bVhCc1qjPEOFKQeh)

🐙 **GitHub Discussions** - Ask questions, share ideas
🔗 [Join Discussions](https://github.com/itskiranbabu/rendercv-enhanced/discussions)

💼 **LinkedIn** - Professional networking
🔗 [Connect on LinkedIn](https://linkedin.com/in/itskiranbabu)

### Get Help

- **Documentation** - Check our [comprehensive docs](DOCUMENTATION.md)
- **FAQ** - See [frequently asked questions](FAQ.md)
- **Issues** - [Search existing issues](https://github.com/itskiranbabu/rendercv-enhanced/issues)
- **Discussions** - [Ask the community](https://github.com/itskiranbabu/rendercv-enhanced/discussions)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### Original RenderCV

This is an enhanced version of [RenderCV](https://github.com/rendercv/rendercv) by Sina Atalay.

Original RenderCV is also licensed under MIT License.

---

## 🙏 Acknowledgments

### Original Creator

**Huge thanks to [Sina Atalay](https://github.com/sinaatalay)** for creating the amazing RenderCV tool that makes CV creation so simple and elegant.

### Contributors

Thank you to all contributors who have helped enhance this project!

### Resources

- **Original RenderCV** - [github.com/rendercv/rendercv](https://github.com/rendercv/rendercv)
- **Typst** - [typst.app](https://typst.app)
- **Python** - [python.org](https://python.org)
- **AI Learning Resources** - Various educators and platforms

### Community

Special thanks to:
- AI Innovators & Agile Leaders Hub community
- All users providing feedback and suggestions
- Open-source contributors worldwide

---

## 📊 Project Stats

![GitHub Stars](https://img.shields.io/github/stars/itskiranbabu/rendercv-enhanced?style=social)
![GitHub Forks](https://img.shields.io/github/forks/itskiranbabu/rendercv-enhanced?style=social)
![GitHub Issues](https://img.shields.io/github/issues/itskiranbabu/rendercv-enhanced)
![GitHub Pull Requests](https://img.shields.io/github/issues-pr/itskiranbabu/rendercv-enhanced)
![Last Commit](https://img.shields.io/github/last-commit/itskiranbabu/rendercv-enhanced)

---

## 🗺️ Roadmap

### Upcoming Features

- [ ] Web-based CV editor
- [ ] More professional themes
- [ ] AI-powered CV suggestions
- [ ] Integration with job boards
- [ ] Mobile app
- [ ] Collaborative editing
- [ ] Version history
- [ ] Export to more formats

### In Progress

- [x] Enhanced documentation
- [x] AI learning resources
- [x] Best practices guide
- [x] Community building

---

## 💬 Feedback

We'd love to hear from you!

- **Feature Requests** - [Open an issue](https://github.com/itskiranbabu/rendercv-enhanced/issues/new?template=feature_request.md)
- **Bug Reports** - [Report a bug](https://github.com/itskiranbabu/rendercv-enhanced/issues/new?template=bug_report.md)
- **General Feedback** - [Start a discussion](https://github.com/itskiranbabu/rendercv-enhanced/discussions)
- **Email** - itskeyrun.ai@gmail.com

---

## 🌟 Star History

[![Star History Chart](https://api.star-history.com/svg?repos=itskiranbabu/rendercv-enhanced&type=Date)](https://star-history.com/#itskiranbabu/rendercv-enhanced&Date)

---

<div align="center">

## 🚀 Ready to Create Your Professional CV?

**[Get Started Now](#-quick-start)** | **[View Examples](#-examples)** | **[Join Community](#-community)**

---

**Made with ❤️ by [itskiranbabu](https://github.com/itskiranbabu)**

**Powered by KeyRun AI**

⭐ **Star this repo if you find it helpful!** ⭐

---

**Connect with me:**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-itskiranbabu-blue?style=flat&logo=linkedin)](https://linkedin.com/in/itskiranbabu)
[![GitHub](https://img.shields.io/badge/GitHub-itskiranbabu-black?style=flat&logo=github)](https://github.com/itskiranbabu)
[![Email](https://img.shields.io/badge/Email-itskeyrun.ai@gmail.com-red?style=flat&logo=gmail)](mailto:itskeyrun.ai@gmail.com)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Community-green?style=flat&logo=whatsapp)](https://whatsapp.com/channel/0029VbCCj7FGJP8EeBLXzD1C)

</div>
