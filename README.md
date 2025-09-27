# Updated EcoCharge Website & JSON Content Manager - Documentation

## 📋 Overview

EcoCharge is a comprehensive website focused on Pakistan's transition to electric vehicles and clean air solutions. The project includes a JSON Content Manager tool for easily managing all dynamic content across the website.

## 🌐 Website Structure

### Pages
- **index.html** - Homepage with EV charging information, carbon calculator, and company overview
- **blog.html** - Blog section displaying articles about Pakistan's electric future
- **research.html** - Research hub with academic papers and studies
- **cleanair.html** - Clean air solutions and filtration technologies
- **map.html** - Interactive EV charging station map
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

### Charging Stations JSON (`map.json`)
```json
[
  {
    "id": 1,
    "name": "Station Name",
    "coords": [24.9689, 67.1687],
    "details": "Station details and rating",
    "fullContent": "<h3>Station Details</h3><p>Full station information</p>",
    "googleMapsLink": "https://maps.google.com/...",
    "kw": 50,
    "chargeTime": "20-45 minutes"
  }
]
```

## 🛠️ JSON Content Manager Tool

### Enhanced Features
- **Multi-Format Support**: Handles blog posts, research papers, AND charging station data
- **Smart Type Detection**: Automatically detects content type (blog/research/map)
- **Upload/Paste JSON**: Load existing JSON files or paste JSON content directly
- **Visual Rich Text Editor**: WYSIWYG editor for HTML content
- **Dynamic Form Fields**: Form adapts based on content type
- **Search & Filter**: Real-time search through all content
- **Export Functionality**: Download updated JSON files with timestamp
- **Responsive Design**: Works on desktop and mobile devices
- **Delete Capability**: Remove unwanted entries safely

### How to Use

1. **Access the Tool**: Visit https://tool-for-jsons-eco-charge.vercel.app/

2. **Load Your JSON**:
   - Upload a JSON file using the file input, OR
   - Paste your JSON content directly into the textarea
   - The tool automatically detects the content type

3. **Edit Content**:
   - Click "Edit" on any card to modify its content
   - Form fields automatically adjust based on content type:
     - **Blog**: Title, author, date, image URL, excerpt, full content
     - **Research**: Title, author, date, categories, excerpt, full content
     - **Map**: Station name, coordinates, details, power, charge time, full content
   - Use the rich text editor for HTML content

4. **Manage Content**:
   - Use search to filter items
   - Delete unwanted entries
   - View statistics (item count, content type, last update)

5. **Save Changes**:
   - Click "Save" to update the entry
   - Use "Export JSON" to download the updated file with timestamp

6. **Integration**:
   - Replace your existing JSON files with the exported content
   - The website will automatically display the updated content

## 🎨 Design System

### Color Palette
- **Primary Green**: `#10b981`
- **Primary Dark**: `#059669`
- **Secondary Teal**: `#0ea5a9`
- **Dark Blue**: `#0f172a`
- **Light Gray**: `#f8fafc`
- **Medium Gray**: `#64748b`
- **Light Border**: `#cbd5e1`
- **White**: `#ffffff`

### Typography
- **Font Family**: Segoe UI system font stack
- **Consistent spacing** with CSS custom properties
- **Card-based layouts** throughout the application
- **Smooth transitions** and hover effects

### Components
- **Cards**: Consistent card design with shadows and rounded corners
- **Modals**: Clean modal windows for editing content
- **Buttons**: Gradient buttons with hover effects
- **Forms**: Styled form controls with focus states
- **Navigation**: Responsive navigation with mobile hamburger menu

## 🔧 Technical Implementation

### Dynamic Content Loading
- All dynamic pages use JavaScript to fetch and display JSON content
- **blog.html**: Fetches and displays blog posts from `blog-posts.json`
- **research.html**: Fetches research papers from `research-papers.json` with search functionality
- **map.html**: Loads charging station data from `map.json` with interactive filtering

### Interactive Features
- **Carbon Calculator**: Real-time CO₂ savings calculator on homepage
- **Interactive Maps**: Leaflet.js integration for charging station maps
- **Modal Systems**: Content preview in modal windows
- **Search & Filter**: Real-time content filtering
- **Mobile Navigation**: Hamburger menu for mobile devices

### Responsive Design
- Mobile-first approach with breakpoints at 768px and 992px
- Flexible grid layouts using CSS Grid and Flexbox
- Optimized touch targets for mobile devices
- Responsive typography and spacing

## 📁 Complete File Structure
```
project-folder/
├── index.html              # Homepage
├── blog.html               # Blog page
├── research.html           # Research hub
├── cleanair.html           # Clean air solutions
├── map.html                # Charging station map
├── test.html               # JSON Content Manager tool
├── blog-posts.json         # Blog content data
├── research-papers.json    # Research papers data
├── map.json                # Charging stations data
├── assets/                 # Optional folder for images
│   ├── images/
│   └── icons/
└── README.md               # This documentation file
```

## 🚀 Deployment Notes

### Prerequisites
1. **Web Server**: Basic web hosting with support for static files
2. **JSON Files**: Ensure all JSON files are in the same directory as HTML files
3. **HTTPS**: Recommended for full functionality (especially geolocation)

### Configuration
1. **CORS Settings**: If hosting JSON files on a different domain, configure CORS headers
2. **API Keys**: Map functionality may require API keys for additional services
3. **Cache Settings**: Configure appropriate caching for JSON files

### Best Practices
- Regular backups of JSON files before making changes
- Version control for content changes
- Testing on multiple devices and browsers
- Monitoring for JSON file errors

## 🔄 Content Update Workflow

### Standard Workflow
1. **Access Tool**: Open the JSON Content Manager
2. **Load Data**: Upload or paste your JSON content
3. **Edit Content**: Modify entries using the intuitive interface
4. **Preview Changes**: Use the rich text editor for HTML content
5. **Export Data**: Download the updated JSON file
6. **Deploy Changes**: Replace the JSON file on your server
7. **Verify**: Check the website to ensure content displays correctly

### Advanced Workflow
1. **Batch Editing**: Use the search feature to find specific content
2. **Content Archiving**: Maintain previous versions of JSON files
3. **Scheduled Updates**: Plan content updates in advance
4. **Multi-format Management**: Handle different content types simultaneously

## 🆕 New Features in Updated JSON Manager

### Enhanced Content Type Support
- **Blog Posts**: Full support for blog content with images
- **Research Papers**: Category management and academic content
- **Map Stations**: Geographic coordinates and charging specifications

### Improved User Experience
- **Real-time Search**: Instant filtering of content
- **Visual Feedback**: Hover effects and transitions
- **Statistics Dashboard**: Item counts and update timestamps
- **Responsive Design**: Mobile-optimized interface

### Advanced Editing Capabilities
- **Rich Text Editor**: WYSIWYG HTML editing
- **Dynamic Forms**: Context-aware form fields
- **Data Validation**: Input validation for different field types
- **Bulk Operations**: Multiple item management

## 📞 Support & Troubleshooting

### Common Issues
- **JSON Format Errors**: Ensure valid JSON syntax
- **File Path Issues**: Verify JSON files are in correct location
- **CORS Errors**: Check server configuration for cross-origin requests
- **Content Display**: Verify all required fields are present

### Troubleshooting Steps
1. **Check Console**: Browser developer tools for error messages
2. **Validate JSON**: Use JSON validators for syntax checking
3. **Test URLs**: Verify JSON files are accessible via direct URL
4. **Clear Cache**: Refresh with cache clearing (Ctrl+F5)

### Getting Help
- Review this documentation thoroughly
- Check JSON file structure against examples provided
- Test with sample data before implementing changes
- Contact support for persistent issues

## 🔮 Future Enhancements

### Planned Features
- **Image Management**: Built-in image upload and management
- **Content Scheduling**: Future-dated content publication
- **User Roles**: Different permission levels for content editors
- **Backup System**: Automated backup of JSON files
- **Analytics Integration**: Content performance tracking

### Technical Roadmap
- **API Version**: REST API for content management
- **Database Integration**: Optional database backend
- **Real-time Updates**: WebSocket-based live updates
- **Progressive Web App**: Offline functionality
