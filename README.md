# 🚗 Car Showroom Website

A comprehensive, modern car showroom website built with PHP, MySQL, HTML, CSS, and JavaScript.

## Features

### Frontend Pages
- ✅ **Homepage** - Hero banner, featured cars, offers, testimonials
- ✅ **Car Listings** - Browse all cars with search and filter options
- ✅ **Car Details** - Detailed car information with EMI calculator
- ✅ **About Us** - Showroom history, mission, vision, team
- ✅ **Services** - All services offered (sales, financing, insurance, servicing, accessories, roadside assistance)
- ✅ **Contact Us** - Contact form, map, business hours, WhatsApp link
- ✅ **Gallery** - Showroom, cars, events, deliveries
- ✅ **Testimonials** - Customer reviews and ratings

### Admin Panel
- ✅ **Dashboard** - Statistics and overview
- ✅ **Car Management** - Add, edit, delete cars
- ✅ **Booking Management** - View and manage bookings
- ✅ **Enquiry Management** - View and manage customer enquiries
- ✅ **Testimonial Management** - Add, edit, delete testimonials

### Additional Features
- ✅ Search and filter cars
- ✅ EMI calculator
- ✅ Responsive design
- ✅ Modern UI/UX
- ✅ Form validation
- ✅ Booking and enquiry forms
- ✅ Test drive request

## Installation

### Requirements
- XAMPP (or any PHP/MySQL server)
- PHP 7.4 or higher
- MySQL 5.7 or higher

### Setup Steps

1. **Clone or download the project**
   ```bash
   cd C:\xampp\htdocs\Car_Web
   ```

2. **Database Setup**
   - The database will be created automatically on first run
   - Database name: `car_showroom`
   - Default admin credentials:
     - Username: `admin`
     - Password: `admin123`

3. **Start XAMPP**
   - Start Apache and MySQL services in XAMPP Control Panel

4. **Access the Website**
   - Frontend: `http://localhost/Car_Web/`
   - Admin Panel: `http://localhost/Car_Web/admin/login.php`

5. **Add Sample Data (Optional)**
   - Run the SQL script in `sample-data.sql` to add sample cars and testimonials
   - Or use the admin panel to add cars manually

## Project Structure

```
Car_Web/
├── admin/              # Admin panel files
│   ├── login.php
│   ├── index.php       # Dashboard
│   ├── cars.php        # Manage cars
│   ├── car-add.php     # Add new car
│   ├── car-edit.php    # Edit car
│   ├── bookings.php    # Manage bookings
│   ├── enquiries.php   # Manage enquiries
│   ├── testimonials.php # Manage testimonials
│   └── logout.php
├── assets/
│   ├── css/
│   │   └── style.css   # Main stylesheet
│   ├── js/
│   │   └── main.js     # Main JavaScript
│   └── images/         # Image assets (create this folder)
├── config/
│   ├── config.php      # Site configuration
│   └── database.php    # Database connection
├── includes/
│   ├── header.php      # Site header
│   └── footer.php      # Site footer
├── index.php           # Homepage
├── cars.php            # Car listings
├── car-details.php     # Car details page
├── about.php           # About us page
├── services.php        # Services page
├── contact.php         # Contact page
├── gallery.php         # Gallery page
├── testimonials.php    # Testimonials page
├── process-booking.php # Process booking form
├── process-enquiry.php # Process enquiry form
├── process-testdrive.php # Process test drive form
└── README.md           # This file
```

## Database Tables

- `cars` - Car inventory
- `bookings` - Customer bookings
- `enquiries` - Customer enquiries
- `testimonials` - Customer testimonials
- `admin_users` - Admin users

## Default Admin Credentials

- **Username:** admin
- **Password:** admin123

⚠️ **Important:** Change the default password after first login!

## Features in Detail

### Car Management
- Add cars with all details (name, model, year, price, specifications, features, images)
- Edit existing cars
- Delete cars
- Multiple images per car
- Car status (available, sold, reserved)

### Booking System
- Customers can book cars
- Request test drives
- Admin can view and manage bookings
- Status tracking (pending, confirmed, cancelled)

### Enquiry System
- Contact form for general enquiries
- Enquiry management in admin panel
- Status tracking (new, read, replied)

### Testimonials
- Add customer testimonials
- Star ratings
- Customer photos
- Show/hide testimonials

## Customization

### Change Site Name
Edit `config/config.php`:
```php
define('SITE_NAME', 'Your Showroom Name');
```

### Change Database Settings
Edit `config/database.php`:
```php
define('DB_HOST', 'localhost');
define('DB_USER', 'root');
define('DB_PASS', '');
define('DB_NAME', 'car_showroom');
```

### Change Contact Information
Edit `includes/footer.php` and `contact.php` to update:
- Address
- Phone numbers
- Email addresses
- WhatsApp number
- Business hours

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## Technologies Used

- **Frontend:** HTML5, CSS3, JavaScript
- **Backend:** PHP 7.4+
- **Database:** MySQL
- **Icons:** Font Awesome 6.4.0
- **Design:** Custom responsive design

## Security Notes

- Passwords are hashed using PHP's `password_hash()`
- SQL injection protection using prepared statements
- XSS protection using `htmlspecialchars()`
- Session management for admin authentication

## Future Enhancements

- User registration and login
- Wishlist functionality
- Car comparison feature
- Advanced search filters
- Email notifications
- Payment gateway integration
- Multi-language support
- Blog section
- Newsletter subscription

## Support

For issues or questions, please contact the development team.

## License

This project is open source and available for educational purposes.

---

**Developed with ❤️ for Car Showroom Management**

