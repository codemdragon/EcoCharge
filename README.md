# EcoCharge Website & JSON Content Manager - Documentation

## 📋 Overview

EcoCharge is a comprehensive website focused on Pakistan's transition to electric vehicles and clean air solutions. The project includes a JSON Content Manager tool for easily managing blog posts and research papers.

## 🌐 Website Structure

### Pages
- **index.html** - Homepage with EV charging information, carbon calculator, and company overview
- **blog.html** - Blog section displaying articles about Pakistan's electric future
- **research.html** - Research hub with academic papers and studies
- **cleanair.html** - Clean air solutions and filtration technologies
- **test.html** - JSON Content Manager tool (hosted at: https://tool-for-jsons-eco-charge.vercel.app/)

## 📊 JSON File Structure

### Blog Posts JSON (`blog-posts.json`)
```json
[
  {
    "id": 1,
    "title": "Blog Post Title",
    "author": "Author Name",
    "date": "Month Day, Year",
    "image": "image-url.jpg",
    "excerpt": "Short description of the blog post...",
    "fullContent": "<p>Full HTML content of the blog post</p>"
  }
]
```

### Research Papers JSON (`research-papers.json`)
```json
[
  {
    "id": 1,
    "title": "Research Paper Title",
    "author": "Author Name",
    "date": "Month Day, Year",
    "categories": ["Category1", "Category2"],
    "excerpt": "Short description of the research...",
    "fullContent": "<p>Full HTML content of the research paper</p>"
  }
]
```

## 🛠️ JSON Content Manager Tool

### Features
- **Upload/Paste JSON**: Load existing JSON files or paste JSON content directly
- **Visual Editing**: Rich text editor for content creation
- **Type Detection**: Automatically detects whether content is for blog or research
- **Export Functionality**: Download updated JSON files
- **Responsive Design**: Works on desktop and mobile devices

### How to Use

1. **Access the Tool**: Visit https://tool-for-jsons-eco-charge.vercel.app/

2. **Load Your JSON**:
   - Upload a JSON file using the file input, OR
   - Paste your JSON content directly into the textarea

3. **Edit Content**:
   - Click "Edit" on any card to modify its content
   - Use the rich text editor for full content
   - Fields automatically adjust based on content type (blog/research)

4. **Save Changes**:
   - Click "Save" to update the entry
   - Use "Export JSON" to download the updated file

5. **Integration**:
   - Replace your existing `blog-posts.json` or `research-papers.json` files with the exported content
   - The website will automatically display the updated content

## 🎨 Design System

### Color Palette
- **Primary Green**: `#10b981`
- **Primary Dark**: `#059669`
- **Secondary Teal**: `#0ea5a9`
- **Dark Blue**: `#0f172a`
- **Light Gray**: `#f8fafc`

### Typography
- **Font Family**: Segoe UI system font stack
- **Consistent spacing** and **card-based layouts** throughout

## 🔧 Technical Implementation

### Dynamic Content Loading
- Blog and research pages use JavaScript to fetch and display JSON content
- Modal windows for detailed content viewing
- Search functionality on research page

### Responsive Design
- Mobile-friendly navigation
- Flexible grid layouts
- Optimized for various screen sizes

### Interactive Elements
- Carbon calculator on homepage
- Smooth scrolling navigation
- Hover effects and transitions

## 📁 File Structure
```
project-folder/
├── index.html
├── blog.html
├── research.html
├── cleanair.html
├── test.html (JSON manager)
├── blog-posts.json (dynamic content)
├── research-papers.json (dynamic content)
└── assets/ (optional folder for images)
```

## 🚀 Deployment Notes

1. **JSON Files**: Ensure `blog-posts.json` and `research-papers.json` are in the same directory as the HTML files
2. **CORS**: If hosting JSON files on a different domain, configure CORS headers
3. **API Keys**: Map functionality requires API key integration
4. **HTTPS**: For full functionality, deploy with HTTPS

## 🔄 Content Update Workflow

1. Use the JSON Content Manager tool to edit content
2. Export the updated JSON file
3. Replace the existing JSON file on your server
4. Clear cache if necessary
5. Content updates appear immediately on the website

## 📞 Support

For issues with the JSON Content Manager tool or website integration, ensure:
- JSON files are properly formatted
- File paths are correct
- All required fields are present in JSON objects
- Content follows the expected structure

This system provides a user-friendly way to manage dynamic content without requiring technical knowledge of web development.
