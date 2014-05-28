######################################################

Pagayo eCommerce Solutions
www.pagayo.com
support@pagayo.com

Copyright 2012 Pagayo. All rights reserved

######################################################

Magento Theme pt001
http://www.pagayo.com/pt001.html

Software requirements:
Installed Magento Community Edition Version 1.4.2 or higher

######################################################



=======================================================
INSTALLATION STEP 1
=======================================================

Create a full backup of your Magento store.

=======================================================
INSTALLATION STEP 2
=======================================================

Extract the zip file and copy all files to your magento folder.

=======================================================
INSTALLATION STEP 3
=======================================================

Activate the theme from your Admin panel:
Please go to System -> Configuration -> Design -> Themes
Put "pt001" without the quotation marks into Templates, Skin (Images / CSS), Layout and Default

=======================================================
INSTALLATION STEP 4
=======================================================

Configuration of the Homepage layout:
Please go to CMS -> Pages -> home (select home as URL Key)


Under Content -> Content box:
Hide Editor and add this code:
{{block type='core/template' template='pagayo/home.phtml'}}


Under Design -> Page Layout:
Select 1column from the Layout Dropdown


Under Design -> Page Layout:
Add this code Layout Update XML:
<reference name="content">
    <block type="catalog/product_list" name="featured" template="catalog/product/list.phtml">
        <action method="setCategoryId"><category_id>***</category_id></action>
        <action method="setColumnCount"><count>5</count></action>
    </block>
</reference>

Here *** will be any category you want to display on your Homepage.
For example: <category_id>3</category_id>

Click "Save Page".

=======================================================
INSTALLATION STEP 5
=======================================================

Clear all Cache under System -> Cache Management.
Then log out from your Magento backend and log in again.

When you followed all Installation Steps, you should now see the new theme in your store frontend.
In your Admin Panel under CMS -> Static Blocks you will find several new blocks to manage the content in your theme for homepage, header, footer, sidebar etc.




######################################################

DEFAULT CONTENT OF STATIC BLOCKS

NOTE: When working on your content in static blocks, we recommend to always hide the Editor. Otherwise you can get some unwanted results. If you accidentally damaged the code of any static block, you can just copy the original code from the reference below.

######################################################


=======================================================
pt001-footer-social
Follow us
=======================================================

<ul class="social-icons">
	<li><a href="#" title="facebook"><img src="{{media url="wysiwyg/icon-social-facebook.png"}}" alt="facebook"/></a></li>
	<li><a href="#" title="twitter"><img src="{{media url="wysiwyg/icon-social-twitter.png"}}" alt="twitter"/></a></li>
	<li><a href="#" title="googleplus"><img src="{{media url="wysiwyg/icon-social-googleplus.png"}}" alt="googleplus"/></a></li>
	<li><a href="#" title="youtube"><img src="{{media url="wysiwyg/icon-social-youtube.png"}}" alt="youtube"/></a></li>
	<li><a href="#" title="vimeo"><img src="{{media url="wysiwyg/icon-social-vimeo.png"}}" alt="vimeo"/></a></li>
	<li><a href="#" title="pinterest"><img src="{{media url="wysiwyg/icon-social-pinterest.png"}}" alt="pinterest"/></a></li>
</ul>

=======================================================
pt001-footer-box1
Customer Service
=======================================================

<ul>
	<li><a href="{{store url="customer-service"}}">Customer Service</a></li>
	<li><a href="{{store url="sales/guest/form"}}">Orders and Returns</a></li>
	<li><a href="{{store url="customer-service"}}">Shipping and Delivery</a></li>
	<li><a href="{{store url="catalog/seo_sitemap/category"}}">Sitemap</a></li>
</ul>

=======================================================
pt001-footer-box2
About Us
=======================================================

<ul>
	<li><a href="{{store url="about-magento-demo-store"}}">About Us</a></li>
	<li><a href="{{store url="privacy-policy-cookie-restriction-mode"}}">Privacy Policy</a></li>
	<li><a href="{{store url="contacts"}}">Contact Us</a></li>
	<li><a href="{{store url="customer-service"}}">Shopping Infos</a></li>	
</ul>

=======================================================
pt001-footer-box3
New Products
=======================================================

<ul>
	<li><a href="{{store url="#"}}">Textlink</a></li>
	<li><a href="{{store url="#"}}">Textlink</a></li>
	<li><a href="{{store url="#"}}">Textlink</a></li>
	<li><a href="{{store url="#"}}">Textlink</a></li>
</ul>

=======================================================
pt001-footer-box4
Popular
=======================================================

<ul>
	<li><a href="{{store url="#"}}">Textlink</a></li>
	<li><a href="{{store url="#"}}">Textlink</a></li>
	<li><a href="{{store url="#"}}">Textlink</a></li>
	<li><a href="{{store url="#"}}">Textlink</a></li>
</ul>

=======================================================
pt001-footer-box5
My Account
=======================================================

<ul>
	<li><a href="{{store url="customer/account"}}">My Account</a></li>
	<li><a href="{{store url="wishlist"}}">My Wishlist</a></li>
	<li><a href="{{store url="checkout/cart"}}">View Cart</a></li>
	<li><a href="{{store url="checkout"}}">Checkout</a></li>
</ul>

=======================================================
pt001-footer-links
Footer Links
=======================================================

<ul class="links">
	<li class="first"><a href="{{store url="about-magento-demo-store"}}">About Us</a></li>
	<li><a href="{{store url="customer-service"}}">Customer Service</a></li>
	<li><a href="{{store url="contacts"}}">Contact Us</a></li>
	<li><a href="{{store url="catalogsearch/advanced"}}">Advanced Search</a></li>
	<li><a href="{{store url="catalogsearch/term/popular"}}">Search Terms</a></li>
	<li><a href="{{store url="catalog/seo_sitemap/category"}}">Sitemap</a></li>
	<li><a class="link-rss" href="{{store url="rss"}}">RSS</a></li>
	<li><a href="{{store url="sales/guest/form"}}">Orders and Returns</a></li>
	<li class="last privacy"><a href="{{store url="privacy-policy-cookie-restriction-mode"}}">Privacy Policy</a></li>
</ul>

=======================================================
pt001-footer-payments
Footer Payments
=======================================================

<ul class="payment-icons">
	<li><img src="{{media url="wysiwyg/icon-payment-paypal.png"}}" alt="PayPal"/></li>
	<li><img src="{{media url="wysiwyg/icon-payment-visa.png"}}" alt="Visa"/></li>
	<li><img src="{{media url="wysiwyg/icon-payment-mastercard.png"}}" alt="MasterCard"/></li>
	<li><img src="{{media url="wysiwyg/icon-payment-amex.png"}}" alt="Amercian Express"/></li>
	<li><img src="{{media url="wysiwyg/icon-payment-moneybookers.png"}}" alt="Moneybookers"/></li>
</ul>

=======================================================
pt001-header-usp1
Fast Shipping
=======================================================

and easy returns

=======================================================
pt001-header-usp2
Secure Shopping
=======================================================

with fast checkout

=======================================================
pt001-header-usp3
Call Center
=======================================================

0123-456789

=======================================================
pt001-home-slider1
pt001-home-slider1
=======================================================

<a href="{{store url="apple-imac-27-inch-2-9ghz.html"}}"><img src="{{media url="wysiwyg/pt001-home-slider1.jpg"}}"/></a>

=======================================================
pt001-home-slider2
pt001-home-slider2
=======================================================

<a href="{{store url="apple-imac-27-inch-2-9ghz.html"}}"><img src="{{media url="wysiwyg/pt001-home-slider2.jpg"}}"/></a>

=======================================================
pt001-home-slider3
pt001-home-slider3
=======================================================

<a href="{{store url="apple-ipod-touch-32gb-black.html"}}"><img src="{{media url="wysiwyg/pt001-home-slider3.jpg"}}"/></a>

=======================================================
pt001-home-topbox
pt001-home-topbox
=======================================================

<a href="{{store url="software.html"}}"><img src="{{media url="wysiwyg/pt001-home-topbox.jpg"}}"/></a>

=======================================================
pt001-home-box1
pt001-home-box1
=======================================================

<a href="{{store url="apple-mac-mini-2-5ghz-i5.html"}}"><img src="{{media url="wysiwyg/pt001-home-box1.jpg"}}"/></a>

=======================================================
pt001-home-box2
pt001-home-box2
=======================================================

<a href="{{store url="apple-ipad-mini.html"}}"><img src="{{media url="wysiwyg/pt001-home-box2.jpg"}}"/></a>

=======================================================
pt001-home-box3
pt001-home-box3
=======================================================

<a href="{{store url="apple-macbook-pro-15-inch.html"}}"><img src="{{media url="wysiwyg/pt001-home-box3.jpg"}}"/></a>

=======================================================
pt001-banner-left
pt001-banner-left
=======================================================

<div class="block block-banner-left">
	<a href="{{store url="apple-ipad-mini.html"}}"><img src="{{media url="wysiwyg/pt001-banner-left.png"}}"/></a>
</div>

=======================================================
pt001-banner-right
pt001-banner-right
=======================================================

<div class="block block-banner-right">
	<a href="{{store url="apple-imac-27-inch-2-9ghz.html"}}"><img src="{{media url="wysiwyg/pt001-banner-right.png"}}"/></a>
</div>



