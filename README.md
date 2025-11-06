# 🚀 DSA Interview Prep - Landing Page

A stunning, modern landing page for Data Structures and Algorithms interview preparation featuring curated questions from top tech companies.

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## ✨ Features

### 🎯 Core Functionality
- **Interactive Landing Page** - Eye-catching hero section with animated gradients
- **12 Top Tech Companies** - Curated DSA questions from industry leaders
- **Individual Downloads** - Company-specific question sets available for download
- **Smooth Navigation** - Fixed navbar with scroll effects and smooth scrolling
- **Fully Responsive** - Optimized for desktop, tablet, and mobile devices

### 🎨 Design Highlights
- **Glassmorphism UI** - Modern frosted glass effects with backdrop blur
- **Futuristic Aesthetics** - Blue and purple gradient themes with animated backgrounds
- **Interactive Cards** - Hover effects with colored glows for each company
- **Animated Grid Background** - Dynamic moving grid pattern
- **Professional Footer** - Multi-column layout with social links

### 💼 Featured Companies
1. **Google** - Two Sum, Longest Substring, Merge K Lists, etc.
2. **Amazon** - Palindromic Substring, Trapping Rain Water, LRU Cache, etc.
3. **Meta** - Valid Parentheses, Add Two Numbers, Product Array, etc.
4. **Netflix** - Maximum Subarray, Median Stream, Top K Elements, etc.
5. **Apple** - Reverse Linked List, Validate BST, Clone Graph, etc.
6. **Microsoft** - Rotate Array, Trie Implementation, LCA, etc.
7. **Adobe** - 3Sum, Container Water, Coin Change, etc.
8. **Uber** - Meeting Rooms, Ride Sharing Design, Valid Sudoku, etc.
9. **LinkedIn** - Maximum Product, URL Shortener, Rotated Array, etc.
10. **Spotify** - Music Playlist Design, Queue with Stacks, etc.
11. **Oracle** - LFU Cache, Database Schema, Rate Limiter, etc.
12. **Salesforce** - CRM System Design, Word Break, Permutations, etc.

## 🛠️ Technologies Used

- **HTML5** - Semantic markup structure
- **CSS3** - Advanced animations, glassmorphism, gradients
- **Vanilla JavaScript** - Smooth scrolling, navbar effects, download handlers
- **No Dependencies** - Pure HTML/CSS/JS, no frameworks required

## 📦 Installation & Usage

### Quick Start
   ```

2. **Open in Browser**
   ```bash
   # Simply open the HTML file
   open index.html
   # or double-click the file in your file explorer
   ```

3. **That's it!** No build process or dependencies needed.

### File Structure
```
dsa-interview-prep/
├── index.html          # Main HTML file with embedded CSS and JS
├── README.md           # This file
└── assets/            # (Optional) Add your PDF files her
```

## 🎯 Key Components

### Navigation Bar
- Fixed position with blur effect
- Smooth scroll-triggered background change
- Responsive mobile menu button
- Gradient logo with company branding

### Hero Section
- Animated gradient text
- Moving grid background
- Call-to-action buttons
- Pulsating radial gradients

### Company Cards
- Glassmorphism design
- 5 DSA questions per company
- Individual download buttons
- Color-coded glow effects on hover
- Smooth transform animations

### Footer
- Four-column layout
- Quick links and resources
- Social media integration
- Contact information
- Copyright notice

## 🎨 Customization Guide

### Change Colors
```css
/* Primary gradient colors */
background: linear-gradient(135deg, #60a5fa, #a78bfa);

/* Company glow colors */
.company-card:nth-child(1) { --glow-color: #4285f4; } /* Google blue */
```

### Add More Companies
```html
<div class="company-card">
    <div class="company-header">
        <div class="company-icon">X</div>
        <h3 class="company-name">Company Name</h3>
    </div>
    <ul class="questions-list">
        <li>Question 1</li>
        <li>Question 2</li>
        <!-- Add more questions -->
    </ul>
    <button class="download-btn">⬇️ Download PDF</button>
</div>
```

### Modify Questions
Edit the `<ul class="questions-list">` within each company card to add/remove/modify questions.

## 🔧 JavaScript Features

### Scroll Effects
```javascript
// Navbar background on scroll
window.addEventListener('scroll', () => {
    const navbar = document.getElementById('navbar');
    if (window.scrollY > 50) {
        navbar.classList.add('scrolled');
    }
});
```

### Smooth Scrolling
```javascript
// Smooth scroll to sections
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href'))
            .scrollIntoView({ behavior: 'smooth' });
    });
});
```

### Download Handlers
```javascript
// Individual company downloads
document.querySelectorAll('.download-btn').forEach(btn => {
    btn.addEventListener('click', function() {
        const companyName = this.closest('.company-card')
            .querySelector('.company-name').textContent;
        // Add your download logic here
    });
});
```

## 📱 Responsive Breakpoints

- **Desktop**: 1200px and above (full layout)
- **Tablet**: 768px - 1199px (adjusted grid)
- **Mobile**: Below 768px (single column, mobile menu)

## 🚀 Performance Features

- **Pure CSS Animations** - No JavaScript animation libraries
- **Optimized Transforms** - Hardware-accelerated CSS properties
- **Lazy Loading Ready** - Structure supports image lazy loading
- **Minimal Dependencies** - Zero external libraries = fast load times

## 🎓 Learning Resources

This project demonstrates:
- Advanced CSS techniques (glassmorphism, gradients, animations)
- Modern JavaScript (ES6+ features, event handling)
- Responsive design principles
- User experience best practices
- Clean code structure

## 📝 Future Enhancements

- [ ] Add actual PDF generation/download functionality
- [ ] Implement search and filter for questions
- [ ] Add difficulty levels (Easy/Medium/Hard)
- [ ] Include video solution links
- [ ] Add user authentication and progress tracking
- [ ] Create a backend API for dynamic content
- [ ] Implement dark/light theme toggle
- [ ] Add code playground for practice

## 🤝 Contributing

Contributions are welcome! Feel free to:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see below for details:

```
MIT License

Copyright (c) 2025 DSA Interview Prep

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

## 💡 Tips for Use

### For Students
- Use this as a study guide for interview preparation
- Track your progress through each company's questions
- Practice implementing solutions before checking answers

### For Educators
- Use as a teaching resource for DSA courses
- Customize questions based on curriculum
- Add your own company-specific questions

### For Developers
- Fork and customize for your portfolio
- Add real download functionality with PDF generation
- Integrate with backend services for dynamic content

## 🐛 Known Issues

- Download buttons currently show alerts (demo mode)
- Mobile menu button doesn't toggle menu (to be implemented)
- No actual PDF files included (structure ready for integration)

## 📞 Support

- **Email**: sarjan6325@gmail.com(demo)


## 🌟 Acknowledgments

- Inspired by modern SaaS landing pages
- Design patterns from Tailwind CSS and shadcn/ui
- Interview questions curated from LeetCode, HackerRank, and real experiences
- Icons and emojis from Unicode standard

## 📊 Browser Support

- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+
- ⚠️ IE11 (limited support, use modern browser recommended)

---

**Built with 💙 for developers preparing for their dream tech careers**

**Star ⭐ this repo if you find it helpful!**
