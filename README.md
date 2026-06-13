<p align="center">
  <img src="https://anarchain.co/_next/image?url=%2Fpic%2FrabbitCMS_Logo.png&w=256&q=100" width="120" alt="Rabbit CMS Logo" />
</p>

<h1 align="center">Rabbit CMS</h1>

<p align="center">
  <strong>Intelligent CMS & Modular Content Infrastructure</strong>
</p>

<p align="center">
  A fast, modular, SEO-focused CMS and admin panel built by Anarchain for news websites, blogs, academies, and content-commerce platforms.
</p>

<p align="center">
  <a href="https://anarchain.co/en/projects/rabbit-cms">Project Page</a> ·
  <a href="https://anarchain.co">Anarchain</a> ·
  <a href="mailto:info@anarchain.co">Contact</a>
</p>

---

## Overview

Rabbit CMS is an intelligent, fast, and modular content management system designed by **Anarchain** for content-heavy digital platforms.

It is built for websites that need more control, speed, SEO structure, and extensibility than traditional plugin-heavy CMS platforms.

Rabbit is designed for:

- News and media websites
- Specialized blogs
- Educational platforms
- Academies
- Multilingual websites
- Content-commerce platforms
- Crypto and finance media
- Personal brands with heavy content
- Companies that need a custom CMS

---

## The Problem

Many content-heavy websites rely on platforms that become slow, fragile, or difficult to customize as they grow.

Rabbit CMS was designed to solve problems such as:

- Heavy dependency on plugin ecosystems
- Poor performance on large content-heavy websites
- Complex multilingual content management
- Weak SEO and internal linking workflows
- No graph-level visibility of content relationships
- High dependency on expensive external storage
- Limited security and upload validation
- Lack of native support for content, products, subscriptions, and payments in one system

---

## Rabbit's Solution

Rabbit is a content infrastructure platform built around:

- Speed
- Modularity
- SEO
- Security
- Extensibility
- Content relationship intelligence
- Commerce and payment support

Instead of relying on dozens of external plugins, Rabbit defines each capability as an extendable module.

---

## Core Features

### Content Editing & Page Building

- Drag-and-drop page and article editor
- Article, news, page, and landing page management
- Real-time preview
- Text, image, video, gallery, form, quote, code, iframe, and product modules
- Dynamic settings per module
- Responsive editing experience

### SEO & Content Growth

- Real-time SEO analysis
- Title, meta, keyword, and image ALT checks
- Internal linking suggestions
- Content relationship management
- Support for topical authority and content path building
- Structured for large blogs and specialized media

### Graph-Based Content Relationships

Rabbit uses graph-based content modeling to understand relationships between:

- Articles
- Categories
- Tags
- Authors
- Products
- Pages

This helps with:

- Internal linking strategy
- Content isolation detection
- SEO path analysis
- Content relationship visualization

### Users, Roles & Workflow

- User management
- Admin, Author, Editor, and Content Manager roles
- Granular access permissions
- Draft, review, published, and scheduled states
- Content versioning
- Comments and interaction management

### Commerce & Payments

- Digital product sales
- Physical product sales
- Subscription sales
- Crypto payment support
- Order management
- Content-to-product linking

### Media, Files & Performance

- Local file storage
- Fast file delivery with Nginx
- Automatic image and file compression
- Gallery, video, audio, and file management
- Page speed optimization
- Reduced dependency on expensive cloud storage

### Security & Access Control

- JWT authentication
- Role and permission control
- Upload file validation
- Suspicious request filtering
- Route and API access restriction
- Security logging and monitoring

---

## Technical Snapshot

| Area | Technology |
|---|---|
| Backend | Go, Gin |
| Frontend | Next.js, React, Tailwind CSS |
| Editor | React DnD |
| Main Database | MongoDB |
| Content Graph | Neo4j |
| Cache / Sessions | Redis |
| File Delivery | Local Storage + Nginx |
| Auth | JWT |
| Architecture | Modular, extensible, SEO-focused |

---

## High-Level Architecture

```txt
Admin User / Public Visitor
        |
        v
Next.js Admin / Public Website
React · Tailwind · DnD · SSR/SSG
        |
        v
Go / Gin API
REST · JWT · Auth · Modules
        |
        +------------------ MongoDB
        |                   Content documents
        |
        +------------------ Neo4j
        |                   Content relationship graph
        |
        +------------------ Redis
        |                   Cache and sessions
        |
        +------------------ Local Storage + Nginx
                            Images, videos, files
