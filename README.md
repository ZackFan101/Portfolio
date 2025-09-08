Zack Fan — HR × Data Portfolio

This is my personal portfolio website showcasing projects, skills, and experiences at the intersection of Human Resources and Data Analytics.
Built with a single index.html, Tailwind CSS via CDN, and vanilla JavaScript.
Deployed with GitHub Pages.

Live site: https://zackfan101.github.io/Portfolio/

✨ Features

Minimal & Fast: pure HTML + Tailwind CDN (no build tools needed).

Bilingual (EN / 中文): toggle language with one click.

Dynamic Rendering: Projects, Skills, Experience, and Education sections are generated via JavaScript.

Responsive: fully mobile-friendly with glassmorphism styling.

Interactive: WeChat QR modal, smooth reveal animations, resume download.

📂 Repo Structure
/ (repo root)
├─ index.html                 # Main page with all logic
├─ assets/
│  ├─ me.jpg                  # Hero photo
│  ├─ wechat_qr.jpg           # WeChat QR code
│  ├─ Ziqiang_Fan_Resume.pdf  # Resume (downloadable)
│  └─ img/
│     └─ bellabeat-cover.png  # (optional) Project cover images
└─ README.md


Optional:

assets/icons/favicon.ico → website icon

robots.txt / sitemap.xml → for SEO

🚀 Deployment (GitHub Pages)

Push changes to the main branch.

In GitHub: Settings → Pages → Deploy from a branch → main /root.

Access your site at:
https://zackfan101.github.io/Portfolio/

🔧 How to Edit
Links

Edit the LINKS object in index.html:

const LINKS = {
  resume: 'assets/Ziqiang_Fan_Resume.pdf',
  email: 'mailto:zackkkk1@outlook.com',
  linkedin: 'https://linkedin.com/in/ziqiang-fan-672607289',
  github: 'https://github.com/ZackFan101',
  phone: 'tel:+8618519220783',
  wechatQR: 'assets/wechat_qr.jpg',
  projects: {
    bellabeat: 'https://zackfan101.github.io/bellabeat_data_analysis/'
  }
};

Projects

Projects are defined in the I18N object. Example:

items: [
  {
    title:'Bellabeat Smart Device Usage — Data Analysis',
    desc:'Exploratory and descriptive analysis of Fitbit-style activity data. Cleaned in Excel and SQL, analyzed with R/ggplot2. Deliverables: HTML live report + PDF final report.',
    badges:['Excel','SQL','R / ggplot2','RMarkdown'],
    link:LINKS.projects.bellabeat,
    linkLabel:'Live Analysis'
  }
]


For multiple buttons (Live / Repo / PDF), use an actions array and adjust renderProjects() accordingly.

🖼 Assets Checklist

assets/me.jpg → hero photo

assets/wechat_qr.jpg → WeChat QR code

assets/Ziqiang_Fan_Resume.pdf → resume file

assets/img/bellabeat-cover.png → (optional) cover image for Bellabeat

🛠 Tech Stack

HTML5

Tailwind CSS (via CDN)

Vanilla JavaScript

GitHub Pages (hosting)

📄 License

The website code is © Zack Fan.
Feel free to reference the structure, but replace the content/design with your own before publishing.
