# Complete Step-by-Step Guide to Markdown

Since you are building your career in Cloud Engineering, DevOps and AI Automation, learning Markdown is one of the most important skills you can develop.

You should be able to document everything you learn, turn your projects into technical articles, publish them on GitHub, and use Medium and LinkedIn to demonstrate your technical knowledge to recruiters and potential employers.

This guide will take you from understanding Markdown syntax to building a professional technical blogging workflow.

## 1. **Understanding Markdown**
  **What is Markdown**

Markdown is a lightweight markup language used to format plain text into readable documents.

It allows you to write:

- Technical blogs and tutorials.
- Project documentation.
- GitHub README files.
- Installation guides.
- DevOps project documentation.
- Cloud architecture explanations.
- API documentation.
- Notes and learning journals.
- LinkedIn and Medium technical articles.
Markdown files use the .md extension.

For example:

```Plain text
README.md
docker-tutorial.md
linux-commands.md
aws-project.md
jenkins-pipeline.md
terraform-guide.md
```

**Where Markdown is used in the real world**

|Platform/tool	|Markdown use case|
|:---|---:|
|VS Code	|Writing and editing documentation
|GitHub	|README, project documentation, issues
|GitLab	|Repository documentation
|Medium	|Writing and preparing technical articles
|LinkedIn|	Preparing formatted article content
|MkDocs	|Building technical documentation websites

## 2.  **Markdown syntax: Every important command and its use case**

This is your Markdown reference guide. Practise each example inside a .md file in VS Co


**A. Heading**
Headings organise your article into sections.
Syntax:

```markdown

# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```

**Real-world use case:**

```markdown
# My Journey into DevOps Engineering

## Introduction

## What is DevOps?

### Benefits of DevOps

### DevOps Tools

## Conclusion
```

Use one main H1 heading for the article title and H2/H3 headings to organise the content.

**B. Paragraphs and line breaks**
Use paragraphs to explain concepts.

```markdown

DevOps is a combination of development and operations.
It improves collaboration, automation and software delivery.
```

For a line break within the same paragraph, end the line with two spaces or use a blank line to start a new paragraph.

**C. Bold text**
Use bold to emphasise important words.

```markdown
**DevOps is about automation and collaboration.**
```

Example:

**Always automate repetitive task where practical**

**D. Italics**
Use italics to highlight terms or introduce concepts.

```markdown
*Infrastructure as Code*
```

**E. Bold and italics together**

``` markdown
***Continuous Integration and Continuous Delivery***
```

**F. Strikethrough**
Use this when documenting corrections or completed changes.

```markdown
~~Old configuration~~
New configuration
```

**G. Lists**
**Unordered lists**

Use these for items without a particular order.

```markdown
## Tools I Am Learning

- Git
- GitHub
- Jenkins
- Docker
- Kubernetes
- Terraform
- AWS
- Azure
```

**Ordered lists**

Use these for procedures and instructions.

```markdown
## Steps to Install Docker

1. Update your Linux system.
2. Install Docker dependencies.
3. Install Docker Engine.
4. Start the Docker service.
5. Verify the installation.
```

**Nested lists**

Use nested lists when explaining subcategories.

```markdown
## DevOps Tools

- Version Control
  - Git
  - GitHub
- CI/CD
  - Jenkins
  - GitHub Actions
- Containerisation
  - Docker
  - Kubernetes
- Infrastructure as Code
  - Terraform
  ```

**I. Links and hyperlinks**
Use links to reference documentation, tools and tutorials.

```markdown
I used the official
[Docker documentation](https://docs.docker.com/)
to understand containerisation.
```

Real-world example:

```markdown
I used the official
[Docker documentation](https://docs.docker.com/)
to understand containerisation.
```

**J. Images and screenshots**
Images help readers understand your technical work.

```markdown
![Docker Architecture](images/docker-architecture.png)
```

For a screenshot:

```markdown
![Jenkins Pipeline Screenshot](images/jenkins-pipeline.png)
```

Your repository must contain the image at the specified path.

For example:

```markdown
my-devops-blog/
├── images/
│   ├── docker-architecture.png
│   └── jenkins-pipeline.png
└── README.md
```

**K. Code blocks**
This is particularly important for DevOps technical blogs.

Use triple backticks to display code.
**Linux example:**

```bash
sudo apt update
sudo apt upgrade -y
```

**Git example:**

```bash
git init
git add .
git commit -m "Initial commit"
```

**Docker example:**

```dockerfile
FROM nginx:latest

COPY index.html /usr/share/nginx/html/

EXPOSE 80
```

**Python example:**

```python
print("Hello DevOps Engineer")
```

The language after the opening backticks enables syntax highlighting on supported platforms.

**L. Inline code**
Use single backticks when mentioning a command or code inside a sentence.

```bash
Run `git status` to check your working directory.
```

**M. Tables**
Tables are excellent for comparing tools, configurations and results.

```markdown
| Tool | Purpose |
|---|---|
| Git | Version control |
| GitHub | Code hosting |
| Jenkins | CI/CD automation |
| Docker | Containerisation |
| Kubernetes | Container orchestration |
| Terraform | Infrastructure as Code |
```

**N. Blockquotes**

Use blockquotes to highlight important explanations or warnings.

```markdown
> Always test your application before deploying it
> to a production environment.
```

**O. Horizontal lines**
Use horizontal lines to separate sections.

```markdown
---
```

**P. Task references and technical notes**
GitHub supports alerts for documentation.

```markdown
> [!NOTE]
> Docker containers are isolated environments.

> [!TIP]
> Use Docker Compose to manage multiple containers.

> [!WARNING]
> Never expose sensitive credentials in GitHub repositories.

> [!IMPORTANT]
> Always check your configuration before deployment.
```

**Q. HTML inside Markdown**
Some Markdown platforms support HTML elements.

```HTML
<details>
<summary>Click to see the installation commands</summary>

```bash
sudo apt update
sudo apt install nginx -y

```code

Use this for expandable sections in GitHub documentation, but check whether your publishing platform supports the same HTML.

### R. Escape special characters

Use a backslash when you need to display a character literally rather than have Markdown interpret it.

```markdown
\*This is not italic text\*
```

**S. Footnotes**

Useful when you want to add references without interrupting the article.

```markdown
Docker is an open-source containerisation platform.[^1]

[^1]: https://www.docker.com/
```

Footnote support varies by platform.

**T. Automatic table of contents**

For a long article, create a contents section with links

```markdown
## Table of Contents

- [Introduction](#introduction)
- [What is Docker?](#what-is-docker)
- [Docker Architecture](#docker-architecture)
- [Installation](#installation)
- [Conclusion](#conclusion)
```

GitHub generates heading anchors automatically. Be aware that punctuation and duplicate headings can affect the anchor names.
