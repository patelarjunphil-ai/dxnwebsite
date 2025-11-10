# DXN Cadiz Service Center Blogger Template

This is a responsive and feature-rich Blogger template designed for the DXN Cadiz Service Center. It includes a powerful product search, a contact form, a Google Map, a real-time clock, and sections for popular products and categories.

**Note on Dummy Data:** This template file contains hardcoded dummy product data. This allows you to open the `template.xml` file directly in a web browser for a visual preview of the layout. This dummy data will be replaced by your actual blog posts once you upload and apply the theme to your Blogger site.

## Installation

1.  Download the `template.xml` file.
2.  Go to your Blogger dashboard.
3.  Navigate to the "Theme" section.
4.  Click the arrow next to the "Customize" button.
5.  Select "Restore".
6.  Upload the `template.xml` file.

## Features

### Responsive Design
The template is fully responsive and will adapt to any screen size, from mobile phones to desktop computers.

### Real-Time Clock
A real-time clock is displayed in the header, showing the current date and time.

### Recommended Image Sizes

For the best results on both desktop and mobile, it is highly recommended that you upload **square (1:1 aspect ratio) images** for your products, with a resolution of at least **800x800 pixels**. This will ensure your product grid looks clean, professional, and displays high-quality images on all devices.

### Logo

To use an image logo instead of the blog title:

1.  Go to the "Layout" section in your Blogger dashboard.
2.  In the "Header" gadget, select "Edit".
3.  Choose "Image" and upload your logo.

### Navigation Menu

To edit the navigation links:

1.  Go to the "Theme" section.
2.  Click the arrow next to the "Customize" button and select "Edit HTML".
3.  Find the `<nav id='nav-wrapper'>` section.
4.  Modify the links within the `<ul class='main-nav'>` element.

### Product Categories

This section automatically displays all the labels (categories) you use on your posts. Clicking a category button will take you to a page showing all products in that category.

### Search Auto-Suggest

The search bar includes an auto-suggest feature. As you type, a dropdown will appear with product suggestions, including thumbnails, to help you find what you're looking for quickly.

### Product Details Page

When you click on a product, you will be taken to a dedicated product details page with a large image, full description, and price. The template automatically prevents the first image in your post from appearing twice on this page.

### Related Products

At the bottom of each product details page, a "Related Products" section will automatically appear, showing other products from the same category. If no related products are found, this section will be hidden.

### Popular Products

To feature a product in the "Popular Products" section, simply add the label "Popular" to the product post. The template will automatically display the 5 most recent posts with this label. This section only appears on the homepage.

### Creating a Product Post

1.  Create a new post in Blogger.
2.  The post title will be the product name.
3.  The first image in the post will be used as the main product image.
4.  The post snippet will be displayed below the product name on the homepage grid.
5.  To add a price, include a `div` element with the class "price" in the post body. For example:
    ```html
    <div class="price">$25.00</div>
    ```
6.  Add relevant labels to categorize the product.

### "About Us" and "Contact Us" Pages

1.  Go to the "Pages" section in your Blogger dashboard.
2.  Create new pages with the titles "About Us" and "Contact Us".
3.  The content you add to these pages will be displayed automatically.

### Adding a Google Map to the Contact Us Page

1.  Go to Google Maps and get the embed code for your location.
2.  Go to "Theme" > "Edit HTML".
3.  Find the comment `<!-- Google Map embed code will go here -->`.
4.  Replace the comment with your Google Map embed code.

### Configuring the Dynamic Contact Form

This template includes a dynamic contact form that submits data without a page reload. To make it work, you need to connect it to a service like [Formspree](https://formspree.io/).

1.  Sign up for a free Formspree account and create a new form endpoint.
2.  Copy the endpoint URL provided by Formspree.
3.  In your Blogger dashboard, go to **Theme** > **Edit HTML**.
4.  Find the following line in the JavaScript section at the bottom of the template:
    ```javascript
    const action = 'YOUR_FORMSPREE_ENDPOINT'; // User needs to replace this
    ```
5.  Replace `YOUR_FORMSPREE_ENDPOINT` with your actual Formspree endpoint URL.
6.  Save the theme. Your contact form is now live!

### Configuring the Facebook Messenger Chat Plugin

This template includes a floating Facebook Messenger chat widget to allow visitors to contact you easily.

1.  Find your **Facebook Page ID**. You can find this in the "About" section of your Facebook Page.
2.  In your Blogger dashboard, go to **Theme** > **Edit HTML**.
3.  Scroll to the bottom of the template and find this code block:
    ```html
    <div class="fb-customerchat"
      attribution="setup_tool"
      page_id="YOUR_FACEBOOK_PAGE_ID">
    </div>
    ```
4.  Replace `YOUR_FACEBOOK_PAGE_ID` with your actual Facebook Page ID.
5.  Save the theme. The Messenger chat widget will now appear on your blog.
