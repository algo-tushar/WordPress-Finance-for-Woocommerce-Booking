# WP Finance for Woocommerce Booking

## Description
WP Finance Plugin is a comprehensive solution designed to automate the generation of invoices and sales reports for WooCommerce and WooCommerce Bookings. The plugin integrates with Dropbox for backup file storage and ensures that all financial documents are securely stored and easily accessible. This plugin is ideal for businesses looking to streamline their invoicing process and maintain organized financial records.

## Features
1. **Generate Invoice on Booking Completed**: Automatically create invoices whenever a booking is completed in WooCommerce Bookings.
2. **Generate Sales Report Every 3 Days**: Automatically generate a sales report every three days to keep track of your business performance.
3. **Dropbox API Integration**: Store generated invoices and sales reports in Dropbox for secure and reliable backup.
4. **Generate PDF**: Convert invoices and sales reports into PDF format for easy sharing and printing.
5. **Database Management**: Efficiently manage and store data related to invoices and sales reports within the WordPress database.
6. **WooCommerce & WooCommerce Bookings Hooks**: Seamlessly integrate with WooCommerce and WooCommerce Bookings to automate workflows and document generation.

## Installation
1. Download the WP Finance Plugin zip file.
2. Navigate to the Plugins section in your WordPress dashboard.
3. Click on "Add New" and then "Upload Plugin".
4. Choose the downloaded zip file and click "Install Now".
5. After installation, click "Activate Plugin".

## Configuration
1. **Dropbox API Setup**:
    - Create a Dropbox App and generate an access token.
    - Navigate to the plugin settings page in your WordPress dashboard.
    - Enter the Dropbox access token in the respective field.

2. **WooCommerce Integration**:
    - Ensure WooCommerce and WooCommerce Bookings are installed and activated.
    - The plugin will automatically hook into the booking completion event to generate invoices.

3. **Report Interval Configuration**:
    - By default, sales reports are generated every 3 days.
    - You can modify this interval by updating the schedule in the plugin settings page.

## Usage
### Generate Invoice on Booking Completed
- When a booking is completed, the plugin will automatically generate an invoice and save it as a PDF.
- The invoice will be stored in the WordPress database and uploaded to Dropbox.

### Generate Sales Report
- Every three days, the plugin will generate a comprehensive sales report.
- The sales report will be saved as a PDF and stored in the WordPress database and Dropbox.

## Hooks and Filters
### WooCommerce & WooCommerce Bookings Hooks
- The plugin uses the following hooks:
    - `woocommerce_booking_complete`: Triggered when a booking is completed to generate an invoice.
    - `wp_cron`: Used to schedule the generation of sales reports every three days.