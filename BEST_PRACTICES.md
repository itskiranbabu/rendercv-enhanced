# 💡 Best Practices Guide - Professional CV/Resume Writing

**Complete guide to creating an outstanding CV that gets you interviews**

*Curated by [itskiranbabu](https://github.com/itskiranbabu) | Powered by KeyRun AI*

---

## 📋 Table of Contents

1. [Introduction](#introduction)
2. [CV vs Resume](#cv-vs-resume)
3. [Content Best Practices](#content-best-practices)
4. [Formatting Best Practices](#formatting-best-practices)
5. [ATS Optimization](#ats-optimization)
6. [Industry-Specific Tips](#industry-specific-tips)
7. [Common Mistakes](#common-mistakes)
8. [Examples](#examples)
9. [Checklist](#checklist)

---

## Introduction

Your CV/resume is your first impression. It needs to:
- **Grab attention** in 6-10 seconds
- **Showcase achievements** not just responsibilities
- **Pass ATS** (Applicant Tracking Systems)
- **Tell your story** professionally
- **Get you interviews** not just applications

This guide provides industry-standard best practices for creating a professional CV that stands out.

---

## CV vs Resume

### Resume (US Standard)

**Length**: 1-2 pages
**Purpose**: Job applications
**Content**: Work experience, skills, education
**Style**: Concise, achievement-focused
**Best for**: Corporate jobs, tech roles, business positions

### CV (Curriculum Vitae)

**Length**: 2+ pages (no limit)
**Purpose**: Academic positions, research roles
**Content**: Publications, research, teaching, grants
**Style**: Comprehensive, detailed
**Best for**: Academia, research, medical fields

### Which Should You Use?

| Situation | Use |
|-----------|-----|
| US corporate job | Resume |
| US academic position | CV |
| Europe/Asia job | CV |
| Tech/Engineering | Resume |
| Research/Medical | CV |

---

## Content Best Practices

### 1. Contact Information

✅ **Include:**
- Full name
- Professional email (firstname.lastname@email.com)
- Phone number with country code
- LinkedIn profile URL
- GitHub profile (for tech roles)
- Personal website/portfolio (if relevant)
- City, State/Country (optional)

❌ **Don't Include:**
- Full street address
- Date of birth
- Marital status
- Photo (unless required)
- Social security number
- References (say "available upon request")

**Example:**
```yaml
cv:
  name: John Doe
  email: john.doe@email.com
  phone: "+1 234 567 8900"
  website: https://johndoe.com
  location: San Francisco, CA
  
  social_networks:
    - network: LinkedIn
      username: johndoe
    - network: GitHub
      username: johndoe
```

### 2. Professional Summary

**Purpose**: Hook the reader in 2-3 sentences

✅ **Good Summary:**
```
"Experienced Software Engineer with 5+ years building scalable web applications. 
Specialized in Python, React, and cloud technologies. Led teams of 5+ engineers 
and reduced system latency by 40% at Tech Corp."
```

❌ **Bad Summary:**
```
"Hard-working professional seeking opportunities to grow and learn in a 
dynamic environment."
```

**Formula:**
```
[Job Title] with [X years] experience in [Industry/Technology].
Specialized in [Key Skills]. [Major Achievement with numbers].
```

### 3. Work Experience

**Most Important Section** - Spend 60% of your time here

#### Structure

```yaml
experience:
  - company: Company Name
    position: Your Job Title
    location: City, State
    start_date: 2020-01
    end_date: present
    highlights:
      - "Achievement 1 with quantifiable results"
      - "Achievement 2 with impact"
      - "Achievement 3 with technologies used"
```

#### Writing Achievements

**Formula**: Action Verb + Task + Result

✅ **Good:**
- "Led team of 5 engineers to develop microservices architecture, reducing API response time by 40%"
- "Implemented CI/CD pipeline using Jenkins and Docker, decreasing deployment time from 2 hours to 15 minutes"
- "Optimized database queries resulting in 60% faster page load times and improved user satisfaction by 25%"

❌ **Bad:**
- "Responsible for developing features"
- "Worked on the backend"
- "Helped with deployments"

#### Action Verbs by Category

**Leadership:**
- Led, Managed, Directed, Coordinated, Supervised, Mentored, Trained

**Achievement:**
- Achieved, Exceeded, Improved, Increased, Reduced, Optimized, Enhanced

**Technical:**
- Developed, Built, Implemented, Designed, Architected, Engineered, Created

**Analysis:**
- Analyzed, Evaluated, Assessed, Investigated, Researched, Identified

**Communication:**
- Presented, Communicated, Collaborated, Facilitated, Negotiated

#### Quantify Everything

**Before:**
- "Improved system performance"
- "Managed a team"
- "Reduced costs"

**After:**
- "Improved system performance by 40%, handling 1M+ requests daily"
- "Managed team of 8 engineers across 3 time zones"
- "Reduced infrastructure costs by $50K annually through AWS optimization"

### 4. Education

**Structure:**
```yaml
education:
  - institution: University Name
    area: Computer Science
    degree: BS
    start_date: 2016-09
    end_date: 2020-05
    location: City, State
    gpa: "3.8/4.0"  # Include if > 3.5
    highlights:
      - "Dean's List all semesters"
      - "President of Computer Science Club"
      - "Relevant coursework: Machine Learning, Algorithms, Databases"
```

**Tips:**
- List most recent first
- Include GPA if > 3.5
- Mention honors, awards, scholarships
- Add relevant coursework for recent graduates
- Include thesis/dissertation title for advanced degrees

### 5. Skills

**Organize by Category:**

```yaml
skills:
  - label: Programming Languages
    details: Python, JavaScript, TypeScript, Java, Go
  - label: Frameworks & Libraries
    details: React, Node.js, Django, Flask, FastAPI
  - label: Cloud & DevOps
    details: AWS, GCP, Docker, Kubernetes, Terraform
  - label: Databases
    details: PostgreSQL, MongoDB, Redis, Elasticsearch
  - label: Tools & Technologies
    details: Git, CI/CD, Jenkins, Jira, Agile/Scrum
```

**Skill Levels:**

Don't list skill levels (Beginner, Intermediate, Expert) - it's subjective.

Instead, demonstrate proficiency through:
- Years of experience
- Projects completed
- Certifications earned
- Technologies used in work experience

### 6. Projects (Optional but Recommended)

**For:**
- Recent graduates
- Career switchers
- Open-source contributors
- Freelancers

**Structure:**
```yaml
projects:
  - name: E-Commerce Platform
    date: 2023
    highlights:
      - "Built full-stack e-commerce platform using React and Node.js"
      - "Implemented payment processing with Stripe API"
      - "Deployed on AWS with 99.9% uptime"
    url: https://github.com/username/project
```

### 7. Certifications

**Include if Relevant:**

```yaml
certifications:
  - name: AWS Certified Solutions Architect
    date: 2023-06
    url: https://aws.amazon.com/certification/
  - name: Google Cloud Professional Data Engineer
    date: 2023-03
```

**Popular Certifications:**
- **Cloud**: AWS, GCP, Azure
- **Data**: Google Data Engineer, Databricks
- **Security**: CISSP, CEH, Security+
- **Project Management**: PMP, Scrum Master
- **AI/ML**: TensorFlow Developer, Google ML Engineer

---

## Formatting Best Practices

### 1. Length

**Resume:**
- **0-5 years experience**: 1 page
- **5-10 years experience**: 1-2 pages
- **10+ years experience**: 2 pages maximum

**CV:**
- No strict limit
- Typically 2-5 pages
- Include all relevant publications, research, teaching

### 2. Font

**Recommended Fonts:**
- Source Sans 3 (RenderCV default)
- Calibri
- Arial
- Helvetica
- Georgia
- Times New Roman

**Font Sizes:**
- Name: 20-24pt
- Section headers: 12-14pt
- Body text: 10-11pt
- Minimum: 10pt (for readability)

### 3. Margins

**Standard:**
- Top: 0.5-1 inch
- Bottom: 0.5-1 inch
- Left: 0.5-1 inch
- Right: 0.5-1 inch

**RenderCV Default:**
```yaml
design:
  page:
    top_margin: 0.7in
    bottom_margin: 0.7in
    left_margin: 0.7in
    right_margin: 0.7in
```

### 4. Spacing

**Consistent spacing is key:**
- Between sections: 0.3-0.5 inches
- Between entries: 0.2-0.3 inches
- Line spacing: 1.0-1.15

**RenderCV handles this automatically!**

### 5. Bullet Points

✅ **Use bullet points for:**
- Achievements
- Responsibilities
- Skills
- Highlights

❌ **Don't use for:**
- Contact information
- Education degrees
- Certifications

**Format:**
- Start with action verb
- Keep to 1-2 lines
- Use parallel structure
- Be specific and quantifiable

### 6. Dates

**Consistent Format:**

✅ **Good:**
- 2020-01 to 2023-05
- Jan 2020 - May 2023
- January 2020 - May 2023

❌ **Bad:**
- Mixing formats
- 01/2020 - 5/23
- 2020 - 23

**RenderCV Format:**
```yaml
start_date: 2020-01
end_date: 2023-05  # or "present"
```

### 7. Colors

**Professional Colors:**
- Black for body text
- Dark blue/gray for headers
- Subtle accent colors

**RenderCV Default:**
```yaml
design:
  colors:
    body: rgb(0, 0, 0)
    name: rgb(0, 79, 144)
    section_titles: rgb(0, 79, 144)
    links: rgb(0, 79, 144)
```

**Avoid:**
- Bright colors (red, yellow, green)
- Multiple colors
- Colored backgrounds

---

## ATS Optimization

### What is ATS?

**Applicant Tracking System** - Software that:
- Scans and parses resumes
- Extracts information
- Ranks candidates
- Filters applications

**90% of large companies use ATS**

### ATS-Friendly Practices

✅ **DO:**
- Use standard section names (Experience, Education, Skills)
- Include keywords from job description
- Use simple formatting (RenderCV handles this)
- Save as PDF (RenderCV default)
- Use standard fonts
- Avoid tables, images, headers/footers
- Spell out acronyms first time

❌ **DON'T:**
- Use fancy graphics or images
- Put important info in headers/footers
- Use tables for layout
- Use text boxes
- Use unusual section names
- Keyword stuff

### Keyword Optimization

**How to Find Keywords:**

1. **Read job description carefully**
2. **Identify required skills**
3. **Note specific technologies**
4. **Look for repeated terms**
5. **Include in your CV naturally**

**Example Job Description:**
```
"Looking for Python developer with experience in Django, 
REST APIs, PostgreSQL, and AWS. Must have strong problem-solving 
skills and experience with Agile methodologies."
```

**Keywords to Include:**
- Python
- Django
- REST APIs
- PostgreSQL
- AWS
- Problem-solving
- Agile

**Include in CV:**
```yaml
skills:
  - label: Programming
    details: Python, JavaScript, Java
  - label: Frameworks
    details: Django, Flask, FastAPI
  - label: Databases
    details: PostgreSQL, MongoDB, Redis
  - label: Cloud
    details: AWS, Docker, Kubernetes
  - label: Methodologies
    details: Agile, Scrum, Test-Driven Development
```

### ATS Testing

**Test your CV:**
1. Copy text from PDF
2. Paste into plain text editor
3. Check if formatting is preserved
4. Ensure all information is readable

**RenderCV PDFs are ATS-optimized by default!**

---

## Industry-Specific Tips

### Tech/Software Engineering

**Focus On:**
- Technical skills (languages, frameworks, tools)
- Projects and GitHub contributions
- System design and architecture
- Performance improvements
- Team collaboration

**Example:**
```yaml
experience:
  - company: Tech Corp
    position: Senior Software Engineer
    highlights:
      - "Architected microservices platform using Python and Docker, serving 10M+ users"
      - "Reduced API latency by 40% through caching and query optimization"
      - "Led team of 5 engineers in Agile environment"
      - "Implemented CI/CD pipeline reducing deployment time by 60%"

skills:
  - label: Languages
    details: Python, JavaScript, TypeScript, Go
  - label: Frameworks
    details: Django, React, Node.js, FastAPI
  - label: Cloud
    details: AWS (EC2, S3, Lambda), Docker, Kubernetes
```

### Data Science/ML

**Focus On:**
- ML algorithms and techniques
- Data analysis and visualization
- Model deployment
- Business impact
- Tools and libraries

**Example:**
```yaml
experience:
  - company: Data Corp
    position: Data Scientist
    highlights:
      - "Built recommendation system using collaborative filtering, increasing user engagement by 25%"
      - "Developed predictive model with 92% accuracy for customer churn"
      - "Analyzed 10M+ records using Python, pandas, and SQL"
      - "Deployed ML models to production using Docker and AWS SageMaker"

skills:
  - label: ML/AI
    details: TensorFlow, PyTorch, Scikit-learn, Keras
  - label: Data Analysis
    details: Python, pandas, NumPy, SQL
  - label: Visualization
    details: Matplotlib, Seaborn, Tableau, Power BI
```

### Product Management

**Focus On:**
- Product strategy and roadmap
- Cross-functional leadership
- User research and data analysis
- Business impact
- Stakeholder management

**Example:**
```yaml
experience:
  - company: Product Co
    position: Senior Product Manager
    highlights:
      - "Led product strategy for mobile app with 5M+ users"
      - "Increased user retention by 30% through data-driven feature prioritization"
      - "Managed cross-functional team of 15 (engineering, design, marketing)"
      - "Launched 3 major features resulting in $2M additional revenue"

skills:
  - label: Product
    details: Product Strategy, Roadmapping, User Research, A/B Testing
  - label: Analytics
    details: SQL, Google Analytics, Mixpanel, Amplitude
  - label: Tools
    details: Jira, Confluence, Figma, Miro
```

### Academic/Research

**Focus On:**
- Publications and citations
- Research interests
- Grants and funding
- Teaching experience
- Conference presentations

**Example:**
```yaml
sections:
  publications:
    - title: "Deep Learning for Natural Language Processing"
      authors:
        - John Doe
        - Jane Smith
      journal: "Nature Machine Intelligence"
      date: 2023-05
      doi: 10.1038/example
      citations: 45
  
  research_interests:
    - "Natural Language Processing"
    - "Machine Learning"
    - "Computer Vision"
  
  grants:
    - title: "NSF Graduate Research Fellowship"
      amount: "$150,000"
      date: 2022
```

### Design/Creative

**Focus On:**
- Portfolio link (essential!)
- Design tools and software
- Projects and clients
- Design process
- Impact on business

**Example:**
```yaml
cv:
  website: https://portfolio.johndoe.com  # Essential!
  
experience:
  - company: Design Studio
    position: Senior UX Designer
    highlights:
      - "Redesigned mobile app increasing user satisfaction by 40%"
      - "Led design system implementation across 5 products"
      - "Conducted user research with 100+ participants"
      - "Collaborated with engineering team of 10 in Agile sprints"

skills:
  - label: Design Tools
    details: Figma, Sketch, Adobe XD, Photoshop, Illustrator
  - label: Prototyping
    details: Framer, Principle, InVision
  - label: Research
    details: User Interviews, Usability Testing, A/B Testing
```

---

## Common Mistakes

### ❌ Mistake 1: Generic Objective Statement

**Bad:**
```
"Seeking a challenging position where I can utilize my skills 
and grow professionally."
```

**Good:**
```
"Software Engineer with 5+ years building scalable web applications. 
Specialized in Python and React. Reduced system latency by 40% at Tech Corp."
```

### ❌ Mistake 2: Listing Responsibilities Instead of Achievements

**Bad:**
```
- Responsible for developing features
- Worked on the backend
- Attended team meetings
```

**Good:**
```
- Developed 15+ features serving 1M+ users using Python and Django
- Architected backend microservices reducing API response time by 40%
- Led weekly sprint planning with team of 8 engineers
```

### ❌ Mistake 3: No Quantifiable Results

**Bad:**
```
- Improved system performance
- Managed a team
- Reduced costs
```

**Good:**
```
- Improved system performance by 40%, handling 1M+ requests daily
- Managed team of 8 engineers across 3 time zones
- Reduced infrastructure costs by $50K annually through AWS optimization
```

### ❌ Mistake 4: Too Long or Too Short

**Bad:**
- 5 pages for 3 years experience
- 1 page for 15 years experience

**Good:**
- 1 page for 0-5 years
- 2 pages for 5+ years
- Focus on recent and relevant experience

### ❌ Mistake 5: Typos and Grammar Errors

**Always:**
- Proofread multiple times
- Use spell checker
- Have someone else review
- Read out loud
- Check for consistency

### ❌ Mistake 6: Irrelevant Information

**Don't Include:**
- High school (if you have college degree)
- Unrelated jobs (unless recent graduate)
- Personal hobbies (unless relevant)
- References (say "available upon request")
- Salary information

### ❌ Mistake 7: Poor Formatting

**Avoid:**
- Multiple fonts
- Inconsistent spacing
- Colored backgrounds
- Images and graphics (unless design role)
- Tables for layout

**Use RenderCV for perfect formatting!**

### ❌ Mistake 8: Lying or Exaggerating

**Never:**
- Lie about education
- Exaggerate job titles
- Claim skills you don't have
- Fabricate achievements

**Remember:** Everything can be verified!

---

## Examples

### Example 1: Software Engineer (3 years experience)

```yaml
cv:
  name: John Doe
  email: john.doe@email.com
  phone: "+1 234 567 8900"
  location: San Francisco, CA
  
  social_networks:
    - network: LinkedIn
      username: johndoe
    - network: GitHub
      username: johndoe
  
  sections:
    summary:
      - "Software Engineer with 3 years building scalable web applications using Python and React"
      - "Specialized in backend development, API design, and cloud infrastructure"
      - "Reduced API response time by 40% and improved system reliability to 99.9% uptime"
    
    experience:
      - company: Tech Corp
        position: Software Engineer
        location: San Francisco, CA
        start_date: 2021-06
        end_date: present
        highlights:
          - "Developed RESTful APIs using Django serving 1M+ requests daily with 99.9% uptime"
          - "Reduced API response time by 40% through caching and database query optimization"
          - "Implemented CI/CD pipeline using Jenkins and Docker, reducing deployment time from 2 hours to 15 minutes"
          - "Collaborated with team of 8 engineers in Agile environment, delivering features every 2 weeks"
          - "Mentored 2 junior developers in Python best practices and code review"
      
      - company: StartupXYZ
        position: Junior Software Engineer
        location: Remote
        start_date: 2020-06
        end_date: 2021-05
        highlights:
          - "Built React frontend with TypeScript, achieving 95% test coverage"
          - "Integrated third-party APIs (Stripe, SendGrid, Twilio) for payment and communication"
          - "Participated in code reviews and improved code quality by 30%"
    
    education:
      - institution: University of California, Berkeley
        area: Computer Science
        degree: BS
        start_date: 2016-09
        end_date: 2020-05
        location: Berkeley, CA
        gpa: "3.8/4.0"
        highlights:
          - "Dean's List all semesters"
          - "Relevant coursework: Algorithms, Data Structures, Databases, Machine Learning"
    
    skills:
      - label: Programming Languages
        details: Python, JavaScript, TypeScript, SQL
      - label: Frameworks & Libraries
        details: Django, Flask, React, Node.js
      - label: Cloud & DevOps
        details: AWS (EC2, S3, RDS), Docker, Kubernetes, Jenkins
      - label: Databases
        details: PostgreSQL, MongoDB, Redis
      - label: Tools
        details: Git, Jira, Agile/Scrum

design:
  theme: classic
```

### Example 2: Data Scientist (5 years experience)

```yaml
cv:
  name: Jane Smith
  email: jane.smith@email.com
  phone: "+1 234 567 8900"
  location: New York, NY
  
  social_networks:
    - network: LinkedIn
      username: janesmith
    - network: GitHub
      username: janesmith
  
  sections:
    summary:
      - "Data Scientist with 5 years building ML models and data pipelines for Fortune 500 companies"
      - "Specialized in predictive modeling, NLP, and recommendation systems"
      - "Increased revenue by $5M through ML-driven product recommendations"
    
    experience:
      - company: Data Corp
        position: Senior Data Scientist
        location: New York, NY
        start_date: 2021-01
        end_date: present
        highlights:
          - "Built recommendation system using collaborative filtering, increasing user engagement by 25% and revenue by $5M"
          - "Developed predictive model for customer churn with 92% accuracy, saving $2M in retention costs"
          - "Led team of 3 data scientists in building ML pipeline processing 10M+ records daily"
          - "Deployed models to production using Docker and AWS SageMaker with 99.9% uptime"
          - "Presented insights to C-level executives influencing product strategy"
      
      - company: Analytics Inc
        position: Data Scientist
        location: Boston, MA
        start_date: 2019-06
        end_date: 2020-12
        highlights:
          - "Analyzed 50M+ customer records using Python, SQL, and Spark"
          - "Built NLP model for sentiment analysis with 88% accuracy"
          - "Created interactive dashboards in Tableau used by 100+ stakeholders"
          - "Improved model performance by 15% through feature engineering"
    
    education:
      - institution: MIT
        area: Computer Science
        degree: MS
        start_date: 2017-09
        end_date: 2019-05
        location: Cambridge, MA
        highlights:
          - "Thesis: Deep Learning for Natural Language Processing"
          - "GPA: 3.9/4.0"
      
      - institution: Stanford University
        area: Mathematics
        degree: BS
        start_date: 2013-09
        end_date: 2017-05
        location: Stanford, CA
        gpa: "3.8/4.0"
    
    skills:
      - label: Machine Learning
        details: TensorFlow, PyTorch, Scikit-learn, Keras, XGBoost
      - label: Data Analysis
        details: Python, pandas, NumPy, SQL, Spark
      - label: Visualization
        details: Matplotlib, Seaborn, Tableau, Power BI
      - label: Cloud & MLOps
        details: AWS (SageMaker, S3, EC2), Docker, MLflow
      - label: Statistics
        details: Hypothesis Testing, A/B Testing, Regression, Time Series
    
    certifications:
      - name: Google Cloud Professional Data Engineer
        date: 2023-03
      - name: AWS Certified Machine Learning - Specialty
        date: 2022-11

design:
  theme: moderncv
```

---

## Checklist

### Before Submitting

- [ ] **Contact Information**
  - [ ] Professional email
  - [ ] Phone number with country code
  - [ ] LinkedIn profile
  - [ ] GitHub profile (for tech roles)
  - [ ] No personal address

- [ ] **Content**
  - [ ] Professional summary (2-3 sentences)
  - [ ] Work experience in reverse chronological order
  - [ ] Achievements with quantifiable results
  - [ ] Action verbs used
  - [ ] Keywords from job description included
  - [ ] Education section complete
  - [ ] Skills organized by category
  - [ ] No typos or grammar errors

- [ ] **Formatting**
  - [ ] 1-2 pages (resume) or appropriate length (CV)
  - [ ] Consistent font and sizing
  - [ ] Proper spacing and margins
  - [ ] Bullet points for achievements
  - [ ] Consistent date format
  - [ ] Professional colors
  - [ ] PDF format

- [ ] **ATS Optimization**
  - [ ] Standard section names
  - [ ] Keywords included naturally
  - [ ] Simple formatting (no tables, images)
  - [ ] Standard fonts
  - [ ] No headers/footers with important info

- [ ] **Proofreading**
  - [ ] Spell checked
  - [ ] Grammar checked
  - [ ] Read out loud
  - [ ] Someone else reviewed
  - [ ] Consistent tense (past for old jobs, present for current)

- [ ] **Tailoring**
  - [ ] Customized for specific job
  - [ ] Relevant experience highlighted
  - [ ] Keywords from job description
  - [ ] Irrelevant information removed

---

## Additional Resources

### Tools

- **RenderCV** - Perfect CV formatting
- **Grammarly** - Grammar and spell checking
- **Hemingway Editor** - Readability improvement
- **LinkedIn** - Professional networking
- **GitHub** - Code portfolio

### Learning

- **Resume Writing Guides** - [Indeed](https://www.indeed.com/career-advice/resumes-cover-letters)
- **ATS Optimization** - [Jobscan](https://www.jobscan.co/)
- **Interview Prep** - [LeetCode](https://leetcode.com/), [Interview Query](https://www.interviewquery.com/)

### Community

- **WhatsApp Channel** - [Join for daily tips](https://whatsapp.com/channel/0029VbCCj7FGJP8EeBLXzD1C)
- **WhatsApp Group** - [Join for discussions](https://chat.whatsapp.com/IfIKh4bVhCc1qjPEOFKQeh)

---

**Need help with your CV? Join our community or open an issue!**

*Curated by [itskiranbabu](https://github.com/itskiranbabu) | Powered by KeyRun AI*
