# 🌍 Digital Clock - Multiple Time Zones

A beautiful, responsive web application that displays the current time in multiple time zones simultaneously with both analog and digital clock displays.

## ✨ Features

### Core Functionality
- **30+ Time Zones** - Support for major cities worldwide
- **Dual Display** - Each timezone shows:
  - Animated analog clock with hour, minute, and second hands
  - Digital time display (HH:MM:SS format)
  - Current date and day of the week
  - UTC offset display

### User Controls
- **Add/Remove Zones** - Dynamically add or remove timezone clocks from the display
- **Format Toggle** - Switch between 24-hour and 12-hour (AM/PM) time formats
- **Real-Time Updates** - Clocks update automatically every second

### Design
- **Responsive Layout** - Works perfectly on desktop, tablet, and mobile devices
- **Beautiful UI** - Modern gradient background with smooth animations
- **Smooth Transitions** - Fade-in and fade-out animations when adding/removing clocks
- **Hover Effects** - Interactive visual feedback

## 🚀 Getting Started

### Quick Start
1. Open `index.html` in any modern web browser
2. The app loads with 4 default timezones (UTC, New York, London, Tokyo)
3. Explore and customize your timezone display

### Using the Application

**Add a Time Zone:**
1. Click the **"+ Add Time Zone"** button
2. Select a location from the dropdown menu
3. Click **"Add"** to display the clock

**Remove a Time Zone:**
- Click the **"×"** button on any clock card to remove it

**Change Time Format:**
- Click the **"24-Hour Format"** button to toggle between 24-hour and 12-hour (AM/PM) display

## 📁 File Structure

```
Redefining-American-Dream/
├── index.html      # HTML structure
├── styles.css      # CSS styling and responsive design
├── script.js       # JavaScript logic and timezone management
└── README.md       # Documentation (this file)
```

## 🛠️ Technical Details

### Technologies Used
- **HTML5** - Semantic markup
- **CSS3** - Animations, gradients, and responsive design
- **Vanilla JavaScript** - No dependencies, pure JS implementation

### Supported Time Zones
The application includes support for 30+ time zones:
- **North America**: NYC, Chicago, Denver, LA, Anchorage, Honolulu
- **South America**: Mexico City, Buenos Aires, São Paulo
- **Europe**: London, Paris, Cairo, Moscow, Istanbul
- **Asia**: Dubai, New Delhi, Bangkok, Hong Kong, Tokyo, Seoul, Shanghai, Singapore, Jakarta, Manila
- **Oceania**: Sydney, Melbourne, Auckland

### How It Works

1. **Timezone Calculation**: 
   - Current UTC time is calculated
   - Offset is applied based on selected timezone
   - Result is displayed in both analog and digital formats

2. **Analog Clock**: 
   - Hour hand: Completes 360° rotation in 12 hours
   - Minute hand: Completes 360° rotation in 60 minutes
   - Second hand: Completes 360° rotation in 60 seconds

3. **Real-Time Updates**:
   - `setInterval()` updates all clocks every 1000 milliseconds (1 second)
   - Smooth rotation animations provide visual feedback

## 📱 Responsive Design

The application adapts to different screen sizes:
- **Desktop**: Multi-column grid layout for optimal viewing
- **Tablet**: 2-column layout with adjusted spacing
- **Mobile**: Single-column layout with optimized touch targets

## 🎨 Customization

### Change Default Time Zones
Edit the `activeTimezones` array in `script.js`:

```javascript
let activeTimezones = [
    { name: 'UTC', offset: 0 },
    { name: 'New York (EST)', offset: -5 },
    // Add or modify timezones here
];
```

### Add New Time Zones
Add entries to the `timezoneList` array:

```javascript
const timezoneList = [
    { name: 'Your City (TZ)', offset: 0 }, // Offset from UTC
    // ...
];
```

### Modify Colors
Update the CSS gradient in `body` selector and color variables throughout `styles.css`.

## ⚙️ Browser Compatibility

Works in all modern browsers that support:
- ES6 JavaScript
- CSS Grid and Flexbox
- CSS Transforms and Animations

**Tested on:**
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)

## 📝 License

This project is open source and available for personal and commercial use.

## 🤝 Contributing

Feel free to fork, modify, and enhance this project. Some ideas for improvements:
- Add timezone search functionality
- Implement local storage to save user preferences
- Add current weather for each timezone
- Create alarm/timer functionality
- Add more timezone options

## 📧 Support

For issues or suggestions, please create an issue in the repository.

---

**Enjoy tracking time across the globe! 🌍⏰**
