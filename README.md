# CivicTrack - Community Issue Tracker

A modern, responsive web application that empowers communities to report and track local civic issues. Built with Leaflet.js and modern web technologies.

## 🌟 Features

### Core Functionality
- **Interactive Map Interface** - Report issues by clicking directly on the map
- **Multi-Image Support** - Upload up to 5 images per issue report
- **GPS Integration** - Use your current location and filter issues by distance
- **Real-time Status Tracking** - Track issues from Reported → In Progress → Resolved
- **Comprehensive History** - View complete status change timeline for each issue

### User Management
- **Role-based Access** - Separate interfaces for regular users and administrators
- **User Authentication** - Simple login system with demo credentials
- **Content Moderation** - Flag inappropriate content and admin review system

### Advanced Features
- **Smart Filtering** - Filter by category, status, and distance
- **Location Search** - Search for any location worldwide
- **Multiple Map Themes** - Light, Dark, and Satellite themes
- **Responsive Design** - Optimized for both desktop and mobile devices
- **Analytics Dashboard** - Community insights and reporting statistics

## 🚀 Quick Start

### Prerequisites
- Modern web browser with JavaScript enabled
- Internet connection (for map tiles and icons)

### Installation
1. Download the `index.html` file
2. Open it in any modern web browser
3. Start reporting issues!

### Demo Credentials
- **Regular User:** `user` / `password`
- **Admin User:** `admin` / `admin`

## 🎯 Usage Guide

### For Community Members
1. Login with your credentials
2. Click "Report New Issue" to start reporting
3. Click on the map to place the issue location
4. Fill in details:
   - Title and description
   - Category (Roads, Lighting, Water, etc.)
   - Impact radius (1km, 3km, 5km)
5. Upload up to 5 images
6. Submit and track your report's progress

### For Administrators
1. Login with admin credentials
2. Access Admin Panel from the tabs
3. Review flagged content and take appropriate action
4. Monitor community analytics for insights
5. Manage user accounts and content moderation

## 🗺️ Map Features

### Navigation
- **Zoom Controls:** Custom + and - buttons
- **GPS Location:** Use current location button
- **Search:** Find any location by name or address

### Themes
- **Light Theme:** Clean, minimalist interface
- **Dark Theme:** Reduced eye strain for night use
- **Satellite Theme:** Real-world imagery with labels

## 🔧 Technical Details

### Architecture
- **Frontend:** Pure HTML, CSS, and JavaScript
- **Maps:** Leaflet.js with multiple tile providers
- **Storage:** LocalStorage for data persistence
- **Icons:** Font Awesome for UI elements
- **Fonts:** Manrope for modern typography

### Data Structure
```javascript
{
  id: "unique_identifier",
  title: "Issue Title",
  description: "Detailed description",
  category: "Roads|Lighting|Water Supply|Cleanliness|Public Safety|Obstructions",
  status: "Reported|In Progress|Resolved",
  lat: latitude,
  lng: longitude,
  radius: impact_radius_in_km,
  timestamp: ISO_date_string,
  reporter: "username",
  photos: ["base64_image_data"],
  statusHistory: [
    { status: "Reported", timestamp: "ISO_date" },
    { status: "In Progress", timestamp: "ISO_date" }
  ],
  flagCount: 0
}
```

### Browser Compatibility
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## 🛡️ Moderation System

### Community Moderation
- Users can flag inappropriate content
- Reports with 3+ flags are automatically hidden
- Flagged content requires admin review

### Admin Tools
- **Review Flags:** View and manage flagged content
- **Resolve Issues:** Mark flagged issues as resolved
- **Dismiss Flags:** Clear false flags
- **Ban Users:** Remove problematic users and their content
- **Analytics:** Monitor community reporting patterns

## 📊 Analytics

The admin dashboard provides insights into:
- **Top Reported Categories** - Most common issue types
- **Status Distribution** - Current state of all reports
- **Top Contributors** - Most active community members

## 🎨 Customization

### Themes
Modify CSS custom properties in the `:root` and theme classes to customize colors and appearance.

### Map Providers
Change tile layer URLs in the theme definitions to use different map providers.

### Categories
Update the category list in both the HTML and JavaScript to match your community's needs.

## 🔒 Privacy & Data

- All data is stored locally in your browser
- No personal information is shared with external services
- GPS location is optional and requires user permission
- Images are stored as base64 strings in LocalStorage

## 🐛 Troubleshooting

### Common Issues
- **Map not loading:** Check internet connection
- **GPS not working:** Ensure location permissions are granted
- **Images not uploading:** Verify file size and format (JPEG, PNG)
- **Data not saving:** Check if LocalStorage is enabled

### Performance Tips
- Limit image sizes for faster loading
- Clear browser cache if experiencing issues
- Use category filters to manage large numbers of reports

## 📱 Mobile Usage

The application is fully optimized for mobile devices with:
- Touch-friendly interface
- Mobile-optimized controls
- Responsive layout adjustments
- Gesture support for map navigation

## 🔄 Status Workflow

1. **Reported** → New issue submitted by user
2. **In Progress** → Issue acknowledged and being addressed
3. **Resolved** → Issue has been fixed or completed

Each status change is recorded with timestamp for full transparency.

## 📄 License

This project is open source and available for community use.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to improve the platform for your community.

## 📞 Support

For questions or support, please open an issue in the repository.

---

**Built with ❤️ for stronger communities**