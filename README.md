# C2Z Web

เว็บไซต์ส่วนตัวของ **C2Z** สร้างด้วย [Jekyll](https://jekyllrb.com/) และ Markdown

เว็บไซต์นี้ใช้สำหรับเผยแพร่บทความ แนะนำเว็บไซต์ โปรเจกต์ และเรื่องราวต่าง ๆ ที่อยากเก็บไว้บนอินเทอร์เน็ต

🌐 **เว็บไซต์:** https://c2z.top/

---

## ✨ Features

- 🏠 หน้าแรก
- 📝 Blog
- 👤 About
- 🔒 Privacy Policy
- ❌ Custom 404 Page
- 🌙 Dark Theme
- 📱 รองรับการใช้งานบนอุปกรณ์ต่าง ๆ
- 📰 เขียนบทความด้วย Markdown
- 📅 แสดงวันที่เผยแพร่บทความ
- 🔗 Header และ Footer ใช้งานร่วมกันทุกหน้า
- 📡 รองรับ RSS Feed
- 🎨 CSS แยกออกจากเนื้อหาเพื่อให้ง่ายต่อการปรับแต่ง

---

## 🛠️ Built With

- [Jekyll](https://jekyllrb.com/)
- [Ruby](https://www.ruby-lang.org/)
- [Markdown](https://www.markdownguide.org/)
- HTML
- CSS

---

## 📁 Project Structure

```text
C2Z Web/
│
├── _includes/
│   ├── footer.html
│   ├── head.html
│   └── header.html
│
├── _layouts/
│   ├── page.html
│   └── post.html
│
├── _posts/
│   └── YYYY-MM-DD-title.markdown
│
├── assets/
│   └── css/
│       ├── blog-custom.css
│       ├── brands-extended.css
│       ├── brands.css
│       ├── reset.css
│       └── style.css
│
├── images/
│
├── about.md
├── blog.md
├── privacy.md
├── 404.md
├── index.html
├── _config.yml
├── Gemfile
├── Gemfile.lock
└── README.md
```

---

## 🚀 Installation

### 1. ติดตั้ง Ruby

ตรวจสอบว่า Ruby ติดตั้งเรียบร้อยแล้ว:

```bash
ruby -v
```

ตรวจสอบ RubyGems:

```bash
gem -v
```

### 2. ติดตั้ง Jekyll

```bash
gem install jekyll
```

ตรวจสอบ:

```bash
jekyll -v
```

### 3. ติดตั้ง Bundler

```bash
gem install bundler
```

ตรวจสอบ:

```bash
bundle -v
```

---

## 📦 Install Dependencies

เปิด Terminal หรือ PowerShell ภายในโฟลเดอร์โปรเจกต์ แล้วใช้:

```bash
bundle install
```

---

## ▶️ Run Local Server

ใช้คำสั่ง:

```bash
bundle exec jekyll serve
```

จากนั้นเปิดเว็บไซต์ที่:

```text
http://localhost:4000/
```

Jekyll จะสร้างเว็บไซต์ที่สร้างเสร็จแล้วไว้ใน:

```text
_site/
```

---

## 📝 Creating a Post

บทความทั้งหมดอยู่ในโฟลเดอร์:

```text
_posts/
```

ชื่อไฟล์ต้องใช้รูปแบบ:

```text
YYYY-MM-DD-title.md
```

ตัวอย่าง:

```text
2026-08-21-welcome-to-c2z.md
```

---

## ✍️ Post Front Matter

ทุกโพสต์ควรมี Front Matter อยู่ด้านบนของไฟล์:

```yaml
---
layout: post
title: "สวัสดีครับ ผม C2Z 👋"
date: 2026-08-21 20:15:56 +0700
categories: blog
---
```

จากนั้นสามารถเขียนเนื้อหาด้วย Markdown ได้ตามปกติ

ตัวอย่าง:

```markdown
# หัวข้อ

สวัสดีครับ นี่คือบทความของ C2Z

## หัวข้อย่อย

สามารถใช้ **ตัวหนา**

สามารถใช้ *ตัวเอียง*

และสามารถสร้างรายการได้:

- รายการที่ 1
- รายการที่ 2
- รายการที่ 3
```

---

## 🗂️ Categories

สามารถกำหนดหมวดหมู่ของบทความได้:

```yaml
categories: blog
```

หรือหลายหมวดหมู่:

```yaml
categories:
  - blog
  - tutorial
```

---

## 🏷️ Tags

สามารถเพิ่ม Tags ให้กับบทความได้:

```yaml
tags:
  - jekyll
  - markdown
  - tutorial
```

---

## 🖼️ Images

สามารถใส่รูปภาพในบทความได้ด้วย Markdown:

```markdown
![คำอธิบายรูปภาพ](/images/example.png)
```

หรือใช้ HTML:

```html
<img src="/images/example.png" alt="Example">
```

---

## ⚙️ Configuration

การตั้งค่าหลักของเว็บไซต์อยู่ใน:

```text
_config.yml
```

ตัวอย่าง:

```yaml
title: C2Z
description: ที่ไหนสักแห่งบนอินเทอร์เน็ต
url: "https://c2z.top"
```

---

## 🧩 Shared Components

เว็บไซต์ใช้ไฟล์ส่วนกลางเพื่อให้แต่ละหน้ามีรูปแบบเดียวกัน

### Header

```text
_includes/header.html
```

ใช้สำหรับส่วนหัวและเมนูของเว็บไซต์

### Head

```text
_includes/head.html
```

ใช้สำหรับ:

- Page Title
- Meta Description
- Favicon
- CSS
- Fonts
- SEO
- Open Graph

### Footer

```text
_includes/footer.html
```

ใช้สำหรับส่วนท้ายของเว็บไซต์ และสามารถใช้ร่วมกันกับหน้า:

- Home
- Blog
- About
- Privacy
- Posts
- 404

---

## 🎨 CSS

ไฟล์ CSS อยู่ใน:

```text
assets/css/
```

สามารถแก้ไข CSS เพื่อปรับแต่ง:

- สี
- ขนาดตัวอักษร
- Layout
- Links
- Blog
- Responsive Design

โดยแยก CSS ออกจากเนื้อหา Markdown เพื่อให้ง่ายต่อการดูแลเว็บไซต์

---

## 🧪 Local Development

หลังจากแก้ไขเว็บไซต์ สามารถรัน:

```bash
bundle exec jekyll serve
```

แล้วเปิด:

```text
http://localhost:4000/
```

Jekyll จะสร้างเว็บไซต์ใหม่โดยอัตโนมัติเมื่อมีการแก้ไขไฟล์

หากมีการแก้ไข `_config.yml` แนะนำให้หยุด Server แล้วรันใหม่

---

## 🌐 GitHub Pages

โปรเจกต์นี้สามารถใช้งานร่วมกับ GitHub Pages ได้

Repository:

```text
C2ZC.github.io
```

เว็บไซต์:

```text
https://c2zc.github.io/
```

และสามารถใช้ Custom Domain:

```text
https://c2z.top/
```

ได้ตามการตั้งค่า DNS และ GitHub Pages

---

## 📜 Credits

เว็บไซต์นี้พัฒนาขึ้นโดย **C2Z**

โปรเจกต์นี้ใช้ [Jekyll](https://jekyllrb.com/) เป็นระบบสร้างเว็บไซต์แบบ Static Site Generator

ส่วนหนึ่งของโครงสร้างและ CSS ของเว็บไซต์ได้รับการดัดแปลงจาก [LittleLink](https://github.com/sethcottle/littlelink)

LittleLink เป็นโปรเจกต์โอเพนซอร์สที่เผยแพร่ภายใต้ **MIT License**

ต้นฉบับ:
https://github.com/sethcottle/littlelink

เครดิตและเงื่อนไขการใช้งานของโปรเจกต์ต้นฉบับยังคงอยู่ตาม License ของ LittleLink

---

## 👤 C2Z

🌐 Website  
https://c2z.top/

> Somewhere on the internet.