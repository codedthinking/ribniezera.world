# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static website for "Fish Lakes: Knowledge to Die For", the first book in the Ribni Ezera series. The site is a bilingual (English/Hungarian) book landing page with sections for book information, author details, sample chapter signup, and image gallery.

## Architecture

This is a simple static website consisting of:

- **Single HTML file**: `index.html` - Contains the entire website structure and content
- **Embedded CSS**: All styling is contained within `<style>` tags in the HTML file  
- **Embedded JavaScript**: All interactivity is contained within `<script>` tags in the HTML file
- **Assets folder**: `/assets/img/` contains all images used on the site

## Key Features

- **Bilingual support**: Content toggles between English (default) and Hungarian
- **Responsive design**: Mobile-first approach with CSS Grid and Flexbox
- **Email signup form**: Collects emails for sample chapter distribution
- **Image gallery**: Showcases photos from the Rila Mountains setting
- **Modal system**: Success confirmation after email signup

## Development Workflow

Since this is a static site with no build process:

1. **Local development**: Open `index.html` directly in a browser or use a simple HTTP server
2. **Testing**: Check functionality by opening the file locally - no special commands needed
3. **Deployment**: Upload files to any static hosting service

## Content Structure

The site follows this layout pattern:
- Hero section with book title and call-to-action
- About section with book description and features
- Endorsements section (currently with placeholder content)
- Author section with bio and social links
- Email signup section with form handling
- Gallery section with Rila Mountains photos
- Footer with links and credits

## Code Organization

All code is contained in `index.html`:
- CSS custom properties define the color scheme and spacing
- JavaScript handles language switching and form interactions
- Content is duplicated for both languages with `data-lang` attributes
- Images use absolute paths starting with `/assets/img/`

## Language System

The bilingual functionality works through:
- Elements tagged with `data-lang="en"` or `data-lang="hu"`
- JavaScript toggles visibility based on current language
- Placeholder text and form labels also switch languages
- Default language is English

## Styling Approach

- CSS custom properties for consistent theming
- Mobile-first responsive design
- Smooth animations and hover effects
- Focus on readability with serif fonts for headings
- Dark overlay on hero background image for text contrast