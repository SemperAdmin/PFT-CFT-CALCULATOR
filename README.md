# USMC PFT/CFT Calculator

A Progressive Web App (PWA) for calculating United States Marine Corps Physical Fitness Test (PFT) and Combat Fitness Test (CFT) scores based on MCO 6100.13A.

## Features

### PFT Calculator
- **Upper Body Events**: Pull-ups or Push-ups scoring by gender and age group
- **Core Strength**: Plank scoring (gender and age neutral)
- **Cardio Events**: 3-Mile Run or 5,000m Row
- **Altitude Compensation**: Automatic scoring adjustments for tests at 4,500+ feet MSL

### CFT Calculator
- **Movement to Contact (MTC)**: 880-yard sprint scoring
- **Ammunition Lift (AL)**: 30lb ammo can lift repetitions
- **Maneuver Under Fire (MANUF)**: Combat movement course timing

### Scoring Tables
All scoring tables are sourced directly from MCO 6100.13A:
- Table 2-2: Pull-ups and Push-ups (max 100 pts / 70 pts respectively)
- Table 2-4: Plank (gender and age neutral, max 100 pts)
- Table 2-5: 3-Mile Run Sea Level
- Table 2-6: 3-Mile Run Altitude
- Table 2-7: 5,000m Row Sea Level
- Table 2-8: 5,000m Row Altitude

### Classifications
| Classification | Score Range |
|----------------|-------------|
| CG's Excellence | 285-300 |
| Body Comp Incentive | 250-284 |
| 1st Class | 235-249 |
| 2nd Class | 200-234 |
| 3rd Class | 150-199 |
| Failure | Below 150 |

### Additional Features
- **Due Date Tracking**: Automatic countdown to next PFT (June 30) and CFT (December 31) deadlines
- **Score Simulator**: "What-if" analysis to see how performance changes affect total score
- **Age Comparison**: Compare your scores against other age groups
- **Training Recommendations**: Personalized tips based on weakest events
- **Score History**: Track your progress over time with local storage
- **Dark Mode**: Toggle between light and dark themes
- **Offline Support**: Works without internet connection (PWA)
- **Mobile Responsive**: Optimized for both desktop and mobile devices

## Technical Details

### Built With
- HTML5, CSS3, JavaScript (vanilla)
- Progressive Web App (PWA) with Service Worker
- No external dependencies

### Browser Support
- Chrome, Firefox, Safari, Edge (modern versions)
- iOS Safari, Android Chrome

### Installation
1. Visit the app URL in a supported browser
2. Click "Add to Home Screen" when prompted (or use browser menu)
3. The app will be available offline

## Development

### Project Structure
```
PFT-CFT-CALCULATOR/
├── index.html          # Main application (HTML, CSS, JS)
├── service-worker.js   # PWA offline support
├── manifest.json       # PWA manifest
├── icon-192.png        # App icon (192x192)
├── icon-512.png        # App icon (512x512)
└── README.md           # This file
```

### Updating
When making changes to the application:
1. Update the `CACHE_NAME` version in `service-worker.js`
2. This ensures users receive the latest version

## References
- [MCO 6100.13A](https://www.marines.mil/News/Publications/MCPEL/Electronic-Library-Display/Article/899255/mco-610013a/) - Marine Corps Physical Fitness and Combat Fitness Tests

## License
This project is for educational and personal use. Not officially affiliated with the United States Marine Corps.
