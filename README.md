# Project SovereignNAS Status Dashboard

A live status monitoring dashboard for **Project SovereignNAS** - a personal home NAS built from repurposed hardware running TrueNAS SCALE.

## 🌟 Overview

This web dashboard provides real-time monitoring of the SovereignNAS infrastructure, displaying the operational status of all integrated services. The page is automatically updated every 5 minutes by a custom sync script running on the TrueNAS SCALE server.

**Live Demo**: [View Dashboard](https://manveer04.github.io/sovereignnas/)

## 🚀 Project Background

**Project SovereignNAS** is a personal tech initiative that transformed an old HP Compaq dc5700 SFF desktop (Pentium Dual-Core E5200, 4GB RAM) into a fully functional home Network Attached Storage (NAS) solution using TrueNAS SCALE.

### The Problem
- Running out of cloud storage space for family photos and videos
- High costs of cloud storage subscriptions
- Privacy concerns with cloud-based storage solutions
- Need for a reliable backup solution for thousands of family memories

### The Solution
A DIY NAS system built with:
- **Repurposed Hardware**: Old HP Compaq desktop given new life
- **NAS-Grade Storage**: Second-hand drives configured with redundancy
- **Virtual Machine Workaround**: Creative installation method due to BIOS limitations
- **Smart Integrations**: AI-powered media indexing and real-time sync

## 🛠️ Technical Architecture

### Core Infrastructure
- **TrueNAS SCALE**: Primary NAS operating system and storage management
- **Disk Mirroring**: Data redundancy for protection against drive failures
- **UPS Integration**: Automated safe shutdown during power outages

### Integrated Services

| Service | Purpose | Status |
|---------|---------|---------|
| **TrueNAS UI** | Storage manager and system dashboard | ✅ Monitored |
| **Tailscale VPN** | Secure remote access to NAS services | ✅ Monitored |
| **Syncthing** | Real-time phone backup and file synchronization | ✅ Monitored |
| **PhotoPrism** | AI-powered photo library with face detection | ✅ Monitored |
| **Shinobi NVR** | IP camera monitoring and surveillance | ✅ Monitored |

### Automation & Monitoring
- **Telegram Alerts**: Real-time system monitoring notifications
- **Custom Sync Scripts**: Automated status updates every 5 minutes
- **ExifTool Integration**: Metadata restoration from Google Photos
- **Cron Jobs**: Scheduled maintenance and backup tasks

## 🎯 Key Features

### For Users
- **Real-time Status Monitoring**: Live dashboard showing all service states
- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Visual Status Indicators**: Clear online/offline status for each service
- **Interactive Elements**: Hover effects and detailed service descriptions

### For System Administration
- **Automated Updates**: Status refreshed every 5 minutes via sync script
- **Service Health Checks**: Continuous monitoring of all critical services
- **Error Detection**: Immediate alerts when services go offline
- **Historical Tracking**: Status logging for trend analysis

## 🏗️ Technical Implementation

### Frontend Technologies
- **HTML5**: Semantic structure and accessibility
- **CSS3**: Modern styling with animations and responsive design
- **JavaScript**: Interactive elements and dynamic content
- **Vanta.js**: Animated background effects using Three.js
- **Responsive Grid**: Flexible layout adapting to all screen sizes

### Design Features
- **Terminal Aesthetic**: Retro-futuristic design inspired by command terminals
- **Matrix-style Animation**: Dynamic network background visualization
- **Glowing Effects**: CSS drop-shadows and text-shadows for cyberpunk feel
- **Color Scheme**: Dark theme with cyan/green accents for readability

### Backend Integration
- **Custom Sync Script**: Python/Shell script running on TrueNAS
- **Service Health Checks**: API calls and port monitoring
- **JSON Data Exchange**: Structured data format for status updates
- **File-based Updates**: Static file generation for web serving

## 📁 Project Structure

```
sovereignnas-main/
├── index.html              # Main dashboard page
├── logo.png                # SovereignNAS project logo
├── manveer.jpg             # Creator profile photo
├── icons/                  # Service icons directory
│   ├── photoprism.png      # PhotoPrism service icon
│   ├── shinobi.png         # Shinobi NVR service icon
│   ├── syncthing.png       # Syncthing service icon
│   ├── tailscale.png       # Tailscale VPN service icon
│   └── truenas.png         # TrueNAS service icon
└── README.md               # Project documentation
```

## 🎨 Design Philosophy

### Visual Identity
- **Color Palette**: Dark backgrounds (#0a0f1c) with cyan highlights (#00ff9f)
- **Typography**: Monospace fonts (Courier New) for terminal authenticity
- **Icons**: Custom service icons with consistent styling
- **Animations**: Subtle hover effects and background animations

### User Experience
- **Immediate Information**: Status visible at a glance
- **Progressive Disclosure**: Additional details on hover
- **Mobile-First**: Responsive design starting from mobile viewports
- **Accessibility**: High contrast ratios and semantic HTML structure


## 🤖 Sync Script Integration

The dashboard is designed to work with a custom sync script running on the TrueNAS server:

### Script Responsibilities
- **Service Health Checks**: Monitor each service endpoint
- **Status Data Generation**: Create JSON with current service states
- **File Updates**: Update HTML with latest status information
- **Error Handling**: Graceful degradation when services are unavailable

### Update Frequency
- **Automatic Updates**: Every 5 minutes via cron job
- **Manual Refresh**: On-demand updates when needed
- **Failure Recovery**: Retry logic for temporary network issues

## 📊 Monitoring & Analytics

### Service Metrics
- **Uptime Tracking**: Historical availability data
- **Response Times**: Service health and performance
- **Error Rates**: Failure frequency and patterns
- **Resource Usage**: System load and capacity planning

### Dashboard Metrics
- **Page Views**: Dashboard access frequency
- **User Engagement**: Interaction patterns and session duration
- **Device Types**: Desktop vs mobile usage
- **Geographic Access**: Remote access patterns via Tailscale

## 🔒 Security Considerations

### Network Security
- **VPN Access**: Tailscale mesh network for secure remote access
- **Firewall Rules**: Port restrictions and access controls
- **SSL/TLS**: HTTPS encryption for web dashboard
- **Authentication**: Service-level authentication where applicable

### Data Privacy
- **Local Storage**: All data remains on personal infrastructure
- **No Cloud Dependencies**: Independent of external services
- **Access Logging**: Monitoring of dashboard access patterns
- **Backup Encryption**: Secured backup storage and transmission

## 🎓 Learning Outcomes

### Technical Skills Developed
- **NAS Administration**: TrueNAS SCALE configuration and management
- **Network Engineering**: VPN setup and remote access configuration
- **Web Development**: Responsive dashboard design and implementation
- **System Integration**: Connecting multiple services and platforms
- **Automation**: Script development for monitoring and maintenance

### Problem-Solving Experience
- **Hardware Limitations**: BIOS constraints and VM workarounds
- **Storage Management**: Disk mirroring and redundancy strategies
- **Service Integration**: API connections and data synchronization
- **User Interface Design**: Status visualization and user experience

### Contribution Ideas
- Additional service integrations
- Mobile app companion
- Historical data visualization
- Performance metrics dashboard
- Automated alerting system

## 📄 Documentation

### Additional Resources
- [TrueNAS Project Story](https://drive.google.com/file/d/1e5qsplT6q8BjbGqeSYrbHpXhXs9uNn1n/view?usp=sharing) - Complete project documentation
- [YouTube Demo](https://www.youtube.com/watch?v=UcmBHz5QIXc) - Video walkthrough
- [LinkedIn Profile](https://www.linkedin.com/in/manveer04/) - Creator contact

### Related Projects
- **TrueNAS SCALE**: Open-source NAS operating system
- **PhotoPrism**: AI-powered photo management
- **Syncthing**: Peer-to-peer file synchronization
- **Tailscale**: Zero-config VPN mesh networking

## 🏆 Project Impact

### Personal Benefits
- **Cost Savings**: Eliminated cloud storage subscription fees
- **Privacy Control**: Complete ownership of family data
- **Learning Experience**: Hands-on experience with enterprise technologies
- **Family Utility**: Reliable backup and sharing for all family members

### Technical Achievements
- **Hardware Resurrection**: Gave new life to outdated computer
- **Integration Complexity**: Successfully connected 5+ different services
- **Automation Success**: Reliable 24/7 operation with minimal intervention
- **Scalability**: Foundation for future home lab expansion

## 📞 Contact

**Creator**: Manveer Singh  
**LinkedIn**: [manveer04](https://www.linkedin.com/in/manveer04/)  
**Project Status**: Active Development  

---

### 💡 Inspiration

> "More than just a technical build, this project was a hands-on learning experience and a meaningful family upgrade — showing that with curiosity and creativity, even old hardware can power something truly useful."


*This dashboard represents the convergence of necessity, creativity, and technical passion - transforming a family storage challenge into a comprehensive learning journey and practical solution.*