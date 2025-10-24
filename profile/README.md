![Boomerang Logistics Demo](https://github.com/My-Logistics-Store/.github/blob/main/insert.gif)

# Welcome to Boomerang Logistics Portal 🚚  

![Boomerang Logistics](https://img.shields.io/badge/Boomerang-Logistics-blue?style=for-the-badge)
![Laravel](https://img.shields.io/badge/Laravel-8.x-FF2D20?style=for-the-badge&logo=laravel&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-7.3%2B%7C8.0%2B-777BB4?style=for-the-badge&logo=php&logoColor=white)

## 🌟 **About the System**  
**Boomerang Logistics Portal** is a comprehensive **Field Service Management (FSM)** and **Delivery Logistics ERP System** designed to streamline delivery operations for logistics companies across Australia.  

The platform serves as the backbone for **multi-tenant logistics operations**, enabling companies to manage drivers, vehicles, parcels, routes, and client relationships through a unified, powerful web-based portal integrated with mobile applications.

---

## 🚀 **Our Mission**  
**To revolutionize logistics management by providing a complete, integrated solution that optimizes delivery operations, ensures compliance, and delivers real-time visibility across the entire supply chain.**

---

## 🔧 **Core Features**  

### 📦 **Shift & Delivery Management**
- **Shift Scheduling**: Create, assign, and manage delivery shifts for drivers
- **Real-Time Tracking**: Monitor driver locations and shift progress in real-time
- **Route Optimization**: Integrated Google Maps API for optimal delivery routing
- **Parcel Tracking**: Complete lifecycle tracking from pickup to delivery
- **Photo Verification**: Proof of delivery with geolocation and timestamp
- **Missed Shift Management**: Track and manage missed or incomplete shifts

### 👥 **Client & Personnel Management**
- **Multi-Client Support**: Manage multiple clients with individual rate structures
- **Cost Center Management**: Track deliveries by client cost centers
- **Client Base Management**: Organize delivery bases and pickup locations
- **Driver Management**: Complete driver profiles with documents and certifications
- **Personnel Tracking**: Manage rates, reminders, and documentation for all staff

### 🚗 **Vehicle & Asset Management**
- **Fleet Management**: Track vehicles, registrations, and assignments
- **Vehicle Inspections**: Digital inspection forms with photo capture
- **Expense Tracking**: Monitor vehicle operational and maintenance expenses
- **Vehicle Types**: Configure different vehicle types and rates

### 📊 **Financial & Reporting**
- **Automated Billing**: Calculate charges based on client rates and shift data
- **Deduction Management**: Track and apply driver deductions with installment plans
- **Expense Management**: Comprehensive expense tracking and reporting
- **Shift Reports**: Detailed reports with export capabilities (Excel)
- **Attendance Tracking**: Monitor driver attendance and performance
- **Monetization Information**: Track revenue and payments per shift

### 🔐 **Security & Compliance**
- **Role-Based Access Control**: Granular permissions for different user types
- **Induction Management**: Track driver inductions and training
- **Document Management**: Store and manage compliance documents with point system
- **OneDrive Integration**: Secure cloud storage for documents and photos
- **JWT Authentication**: Secure API authentication for mobile apps

### 📱 **Mobile Integration**
- **Driver Mobile App**: Android/iOS apps for drivers to manage shifts and deliveries
- **Offline Capability**: Works in areas with limited connectivity
- **Real-Time Sync**: Automatic synchronization when connection is available
- **Location Tracking**: Background GPS tracking during shifts
- **Digital Signatures**: Capture signatures for inductions and deliveries

### 🗺️ **Advanced Features**
- **Live Tracking Dashboard**: Real-time map view of all active drivers
- **Route Matrix Optimization**: Google Maps Route Matrix API integration
- **Geocoding**: Automatic address resolution from coordinates
- **State-Based Operations**: Manage operations across different Australian states
- **Import/Export**: Bulk operations for shifts, clients, and rates
- **API Throttling**: Rate limiting for API security

---

## 💻 **Technology Stack**  

### **Backend**
- **Framework**: Laravel 8.x
- **Authentication**: Laravel Sanctum + JWT (tymon/jwt-auth)
- **Database**: MySQL/MariaDB
- **Queue System**: Laravel Queue for background jobs

### **Frontend**
- **Framework**: Bootstrap 5.1.3
- **JavaScript**: Vue.js 2.6 + Vanilla JS
- **CSS**: Sass/SCSS
- **Build Tool**: Laravel Mix (Webpack)

### **Third-Party Integrations**
- **Google Maps API**: Route optimization, geocoding, distance matrix
- **OneDrive API**: Document and photo storage
- **Excel Export**: PHPSpreadsheet for data exports
- **CORS**: Fruitcake Laravel CORS for API access

### **DevOps & Tools**
- **Version Control**: Git
- **Deployment**: Rsync-based automated deployment
- **Caching**: Laravel cache system
- **Logging**: Monolog with Laravel logging

---

## 📂 **System Architecture**

### **Main Modules**

1. **Administration**
   - User access management
   - Role and permission configuration
   - System settings and configuration

2. **Shift Management**
   - Shift creation and scheduling
   - Shift approval workflow (Pending → Approved → Paid)
   - Route tracking and mapping
   - Parcel management per shift

3. **Person Management**
   - Driver and staff profiles
   - Rate management per person
   - Document management with reminders
   - Address and contact information

4. **Client Management**
   - Client profiles with ABN/ACN
   - Multiple addresses per client
   - Cost centers and bases
   - Custom rate structures

5. **Vehicle Management**
   - Vehicle registration and details
   - Vehicle types and configurations
   - Assignment tracking

6. **Inspection & Induction**
   - Digital vehicle inspections
   - Driver induction tracking
   - Signature capture
   - Compliance monitoring

7. **Financial Management**
   - Expense tracking (operational and general)
   - Deduction management with installments
   - Automated billing calculations
   - Export for accounting systems

8. **Live Tracking**
   - Real-time driver location
   - Shift status monitoring
   - Map-based visualization

---

## 📱 **Mobile App Integration**

The portal seamlessly integrates with Android and iOS mobile applications:

### **Features Available in Mobile Apps**
- Real-time shift synchronization
- Offline parcel management
- Background GPS tracking
- Photo capture with geolocation
- Digital signature capture
- Route navigation
- Push notifications
- Document viewing and upload

### **API Authentication**
Mobile apps use JWT authentication with automatic token refresh:
- Access tokens (60-minute expiry)
- Refresh tokens (persistent)
- Automatic reauthorization

---

## 🌏 **Multi-State Operations**

The system supports operations across multiple Australian states:
- State-specific configurations
- Client bases per state
- Driver assignments by region
- State-based reporting
- Compliance tracking per jurisdiction

---

## 📊 **Reporting & Analytics**

### **Available Reports**
- **Shift Reports**: Detailed shift information with financial data
- **Attendance Reports**: Driver attendance and performance
- **Expense Reports**: Vehicle and operational expenses
- **Inspection Reports**: Vehicle inspection history
- **Induction Reports**: Driver induction status
- **Deduction Reports**: Driver deduction tracking
- **Client Reports**: Client-specific delivery metrics

### **Export Formats**
- Excel (XLSX) for all major reports
- CSV for data imports
- PDF for document archival (inspections, inductions)

---


## ✨ **Future Roadmap**

- [ ] AI-powered route prediction
- [ ] Customer portal for real-time tracking
- [ ] Advanced analytics dashboard
- [ ] Integration with accounting software (Xero, MYOB)
- [ ] Automated invoicing
- [ ] Electronic Proof of Delivery (ePOD)
- [ ] Driver mobile app enhancement
- [ ] Multi-language support
- [ ] Advanced reporting with BI tools

---

## 📞 **Support & Contact**

For technical support or inquiries:
- 📧 **Email**: support@boomeranglogistics.com.au
- 🌐 **Portal**: https://boomerang.mylogistics.store
- 📱 **Mobile Apps**: Available on Google Play Store and Apple App Store

---

## 📄 **License**

Copyright © Boomerang Logistics. All rights reserved.

This software is proprietary and confidential. Unauthorized copying, distribution, or use of this software, via any medium, is strictly prohibited.
