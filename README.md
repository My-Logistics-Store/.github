![Boomerang Logistics Demo](./insert.gif)

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
- **Language**: PHP 7.3+ | 8.0+
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

## 🔄 **API Endpoints**

### **Authentication**
- `POST /api/login` - Driver login
- `POST /api/signUp` - Driver registration
- `POST /api/forgotPassword` - Password recovery
- `POST /api/changePassword` - Update password

### **Shift Operations**
- `POST /api/addShift` - Create new shift
- `POST /api/shiftStart` - Start a shift
- `POST /api/finishShift` - Complete a shift
- `POST /api/allShift` - Get shift list
- `POST /api/updateShiftTiming` - Update shift times

### **Parcel Operations**
- `POST /api/addParcel` - Add parcel to shift
- `POST /api/deliverParcel` - Mark parcel as delivered
- `POST /api/undeliverParcel` - Mark parcel as undelivered
- `POST /api/routeOptimization` - Optimize delivery route
- `POST /api/allParcel` - Get all parcels for shift

### **Location Tracking**
- `POST /api/addLocation` - Add location point
- `POST /api/trackLocation` - Track driver location
- `POST /api/searchLocation` - Search for addresses

### **Inspection & Induction**
- `GET /api/inspectionRego` - Get vehicle registrations
- `POST /api/addInspection` - Submit vehicle inspection
- `GET /api/allInduction` - Get induction list
- `POST /api/uploadInduction` - Upload induction documents

---

## 🛠️ **Installation & Setup**

### **Prerequisites**
- PHP 7.3+ or PHP 8.0+
- Composer
- MySQL/MariaDB
- Node.js & NPM
- Web server (Apache/Nginx)

### **Installation Steps**

1. **Clone the repository**
```bash
git clone <repository-url>
cd Boomerang-Logistics-Portal
```

2. **Install PHP dependencies**
```bash
composer install
```

3. **Install Node dependencies**
```bash
npm install
```

4. **Environment configuration**
```bash
cp .env.example .env
php artisan key:generate
```

5. **Configure `.env` file**
```env
DB_DATABASE=your_database
DB_USERNAME=your_username
DB_PASSWORD=your_password

GOOGLE_MAPS_API_KEY=your_google_maps_key
JWT_SECRET=your_jwt_secret

ONEDRIVE_CLIENT_ID=your_onedrive_client_id
ONEDRIVE_CLIENT_SECRET=your_onedrive_secret
```

6. **Run migrations**
```bash
php artisan migrate
```

7. **Seed the database (optional)**
```bash
php artisan db:seed
```

8. **Build assets**
```bash
npm run prod
```

9. **Create storage link**
```bash
php artisan storage:link
```

10. **Set permissions**
```bash
chmod -R 775 storage bootstrap/cache
```

---

## 🚀 **Deployment**

### **Using the Safe Deploy Script**

The system includes an automated deployment script for safe production deployments:

```bash
cd /path/to/Boomerang-Logistics-Portal
./deploy-safe.sh
```

**The script automatically:**
- ✅ Verifies server health before deployment
- 💾 Creates automatic backup
- 🔍 Removes problematic files
- 📦 Deploys application files
- 🧹 Clears Laravel cache
- 🧪 Tests the deployment
- 🔄 Automatic rollback on failure

For detailed deployment instructions, see [DEPLOY_INSTRUCTIONS.md](DEPLOY_INSTRUCTIONS.md)

### **Manual Deployment**

If manual deployment is required:

```bash
# Clear cache
php artisan config:clear
php artisan cache:clear
php artisan route:clear
php artisan view:clear

# Optimize for production
php artisan config:cache
php artisan route:cache
php artisan view:cache
```

---

## 🧪 **System Health Check**

Verify system integrity with the built-in health check:

```bash
php artisan system:health-check
```

This checks:
- ✅ Database connectivity
- ✅ Required tables
- ✅ Storage permissions
- ✅ PHP configuration
- ✅ Critical routes
- ✅ Absence of problematic files

---

## 📊 **Database Schema**

### **Key Tables**
- `shifts` - Delivery shift information
- `parcels` - Parcel/package details
- `drivers` - Driver profiles
- `persons` - Personnel information
- `clients` - Client companies
- `client_centers` - Client cost centers
- `client_bases` - Client pickup/delivery bases
- `vehicals` - Vehicle information
- `inspections` - Vehicle inspections
- `inductions` - Driver inductions
- `expenses` - Expense tracking
- `deduction_plans` - Deduction management
- `states` - Australian states
- `track_locations` - GPS tracking data

---

## 🔐 **User Roles & Permissions**

The system supports role-based access control with customizable permissions:

- **Super Admin**: Full system access
- **Admin**: Management access to all modules
- **Manager**: Limited management capabilities
- **Accountant**: Financial module access
- **Driver**: Mobile app access only

Permissions are managed through the Administration module with granular control over:
- Module access
- Create/Edit/Delete operations
- Report generation
- Export capabilities

---

## 📈 **Key Workflows**

### **Typical Delivery Shift Workflow**

1. **Shift Creation** (Admin Portal)
   - Admin creates shift with client, cost center, and driver
   - Assigns vehicle and sets expected dates
   
2. **Shift Acceptance** (Mobile App)
   - Driver receives notification
   - Reviews shift details
   - Starts shift from mobile app

3. **Parcel Management** (Mobile App)
   - Driver adds/scans parcels
   - System optimizes delivery route
   - Driver navigates to delivery points

4. **Delivery Execution** (Mobile App)
   - Captures proof of delivery (photo + signature)
   - Records geolocation and timestamp
   - Marks parcel as delivered/undelivered

5. **Shift Completion** (Mobile App)
   - Driver finishes shift
   - System calculates odometer difference
   - Captures end location

6. **Shift Approval** (Admin Portal)
   - Manager reviews shift details
   - Verifies all parcels accounted for
   - Approves for payment

7. **Payment Processing** (Admin Portal)
   - System calculates charges and pay
   - Applies any deductions
   - Marks shift as paid
   - Exports for accounting

---

## 🛡️ **Security Features**

- **JWT Token Authentication**: Secure API access with refresh tokens
- **Password Encryption**: Bcrypt hashing for all passwords
- **CORS Protection**: Configured cross-origin policies
- **SQL Injection Prevention**: Laravel Query Builder protection
- **XSS Protection**: Input sanitization and output escaping
- **CSRF Protection**: Token-based form protection
- **Rate Limiting**: API throttling (120 requests/minute)
- **Secure File Storage**: OneDrive integration with access controls
- **Audit Logging**: Track critical system changes

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

## 🔧 **Configuration**

### **Google Maps Configuration**
```php
// config/services.php
'google_maps' => [
    'key' => env('GOOGLE_MAPS_API_KEY'),
],
```

### **OneDrive Configuration**
```php
// config/onedrive.php
'client_id' => env('ONEDRIVE_CLIENT_ID'),
'client_secret' => env('ONEDRIVE_CLIENT_SECRET'),
'tenant_id' => env('ONEDRIVE_TENANT_ID'),
```

### **JWT Configuration**
```php
// config/jwt.php
'ttl' => 60, // Token time to live in minutes
'refresh_ttl' => 20160, // Refresh token TTL (2 weeks)
```

---

## 🐛 **Troubleshooting**

### **Common Issues**

#### **Error 500 - Server Error**
```bash
# Clear all caches
php artisan cache:clear
php artisan config:clear
php artisan route:clear
php artisan view:clear

# Check for problematic files
php artisan system:health-check
```

#### **Database Connection Failed**
- Verify `.env` database credentials
- Check MySQL/MariaDB service is running
- Ensure database exists and is accessible

#### **File Upload Issues**
- Check `storage/` permissions (775)
- Verify PHP `upload_max_filesize` and `post_max_size`
- Ensure OneDrive credentials are configured

#### **Google Maps Not Loading**
- Verify `GOOGLE_MAPS_API_KEY` in `.env`
- Check API key permissions in Google Cloud Console
- Enable required APIs: Maps JavaScript API, Geocoding API, Routes API

#### **JWT Token Issues**
```bash
# Regenerate JWT secret
php artisan jwt:secret
```

---

## 📚 **Documentation**

- **API Documentation**: Available at `/api/documentation` (when enabled)
- **Deployment Guide**: [DEPLOY_INSTRUCTIONS.md](DEPLOY_INSTRUCTIONS.md)
- **User Manual**: Contact system administrator
- **Developer Guide**: See inline code documentation

---

## 🔄 **Version Control & Updates**

### **Branches**
- `main` - Production-ready code
- `develop` - Development branch
- `feature/*` - Feature branches
- `hotfix/*` - Critical fixes

### **Update Process**
1. Pull latest changes
2. Review `composer.json` and `package.json` for new dependencies
3. Run `composer install` and `npm install`
4. Execute new migrations
5. Test thoroughly
6. Deploy using safe deploy script

---

## 🤝 **Contributing**

For internal development team:
1. Create feature branch from `develop`
2. Follow PSR-12 coding standards
3. Write descriptive commit messages
4. Test all changes thoroughly
5. Submit pull request with detailed description
6. Ensure CI/CD pipeline passes
7. Request code review from team lead

---

## 🌱 **Sustainability & Best Practices**

At Boomerang Logistics, we promote:
- **Route Optimization**: Reducing fuel consumption through smart routing
- **Digital Documentation**: Paperless operations
- **Efficient Resource Allocation**: Maximizing vehicle and driver utilization
- **Data-Driven Decisions**: Analytics for continuous improvement

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

---

## 🙏 **Acknowledgments**

Built with ❤️ using:
- Laravel Framework
- Bootstrap UI Framework
- Google Maps Platform
- Microsoft OneDrive
- Open source community contributions

---

**Made with precision for logistics excellence across Australia 🇦🇺**
