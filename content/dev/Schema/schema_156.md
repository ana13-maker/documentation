---
title: Zen Cart 1.5.6 Schema 
category: schema 
weight: -156 
---

# Database Schema

[address_book](#address_book)    [address_format](#address_format)    [admin](#admin)    [admin_activity_log](#admin_activity_log)    [admin_menus](#admin_menus)    [admin_notifications](#admin_notifications)    [admin_pages](#admin_pages)    [admin_pages_to_profiles](#admin_pages_to_profiles)    [admin_profiles](#admin_profiles)    [authorizenet](#authorizenet)    [banners](#banners)    [banners_history](#banners_history)    [categories](#categories)    [categories_description](#categories_description)    [configuration](#configuration)    [configuration_group](#configuration_group)    [counter](#counter)    [counter_history](#counter_history)    [countries](#countries)    [coupon_email_track](#coupon_email_track)    [coupon_gv_customer](#coupon_gv_customer)    [coupon_gv_queue](#coupon_gv_queue)    [coupon_redeem_track](#coupon_redeem_track)    [coupon_restrict](#coupon_restrict)    [coupons](#coupons)    [coupons_description](#coupons_description)    [currencies](#currencies)    [customers](#customers)    [customers_basket](#customers_basket)    [customers_basket_attributes](#customers_basket_attributes)    [customers_info](#customers_info)    [db_cache](#db_cache)    [email_archive](#email_archive)    [ezpages](#ezpages)    [ezpages_content](#ezpages_content)    [featured](#featured)    [files_uploaded](#files_uploaded)    [geo_zones](#geo_zones)    [get_terms_to_filter](#get_terms_to_filter)    [group_pricing](#group_pricing)    [languages](#languages)    [layout_boxes](#layout_boxes)    [manufacturers](#manufacturers)    [manufacturers_info](#manufacturers_info)    [media_clips](#media_clips)    [media_manager](#media_manager)    [media_to_products](#media_to_products)    [media_types](#media_types)    [meta_tags_categories_description](#meta_tags_categories_description)    [meta_tags_products_description](#meta_tags_products_description)    [music_genre](#music_genre)    [newsletters](#newsletters)    [orders](#orders)    [orders_products](#orders_products)    [orders_products_attributes](#orders_products_attributes)    [orders_products_download](#orders_products_download)    [orders_status](#orders_status)    [orders_status_history](#orders_status_history)    [orders_total](#orders_total)    [paypal](#paypal)    [paypal_payment_status](#paypal_payment_status)    [paypal_payment_status_history](#paypal_payment_status_history)    [paypal_session](#paypal_session)    [paypal_testing](#paypal_testing)    [product_music_extra](#product_music_extra)    [product_type_layout](#product_type_layout)    [product_types](#product_types)    [product_types_to_category](#product_types_to_category)    [products](#products)    [products_attributes](#products_attributes)    [products_attributes_download](#products_attributes_download)    [products_description](#products_description)    [products_discount_quantity](#products_discount_quantity)    [products_notifications](#products_notifications)    [products_options](#products_options)    [products_options_types](#products_options_types)    [products_options_values](#products_options_values)    [products_options_values_to_products_options](#products_options_values_to_products_options)    [products_to_categories](#products_to_categories)    [project_version](#project_version)    [project_version_history](#project_version_history)    [query_builder](#query_builder)    [record_artists](#record_artists)    [record_artists_info](#record_artists_info)    [record_company](#record_company)    [record_company_info](#record_company_info)    [reviews](#reviews)    [reviews_description](#reviews_description)    [salemaker_sales](#salemaker_sales)    [sessions](#sessions)    [specials](#specials)    [tax_class](#tax_class)    [tax_rates](#tax_rates)    [template_select](#template_select)    [upgrade_exceptions](#upgrade_exceptions)    [whos_online](#whos_online)    [zones](#zones)    [zones_to_geo_zones](#zones_to_geo_zones) 

## address_book

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**address_book_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[customers_id](#customers)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>entry_gender</td>

<td>char(1)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>entry_company</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>entry_firstname</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>entry_lastname</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>entry_street_address</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>entry_suburb</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>entry_postcode</td>

<td>varchar(10)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>entry_city</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>entry_state</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>entry_country_id</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>entry_zone_id</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## address_format

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**address_format_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>address_format</td>

<td>varchar(128)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>address_summary</td>

<td>varchar(48)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## admin

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**admin_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>admin_name</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>admin_email</td>

<td>varchar(96)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>admin_profile</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>admin_pass</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>prev_pass1</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>prev_pass2</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>prev_pass3</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>pwd_last_change_date</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>reset_token</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_login_date</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_login_ip</td>

<td>varchar(45)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>failed_logins</td>

<td>smallint(4) unsigned</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>lockout_expires</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_failed_attempt</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_failed_ip</td>

<td>varchar(45)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## admin_activity_log

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**log_id**

</td>

<td>bigint(15)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>access_date</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[admin_id](#admin)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>page_accessed</td>

<td>varchar(80)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>page_parameters</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>ip_address</td>

<td>varchar(45)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>flagged</td>

<td>tinyint(4)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attention</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>gzpost</td>

<td>mediumblob</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>logmessage</td>

<td>mediumtext</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>severity</td>

<td>varchar(9)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td>info</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## admin_menus

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**menu_key**

</td>

<td>varchar(191)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>language_key</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>sort_order</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## admin_notifications

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**notification_key**

</td>

<td>varchar(40)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[admin_id](#admin)</td>

<td>int(11)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>dismissed</td>

<td>char(1)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## admin_pages

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**page_key**

</td>

<td>varchar(191)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>language_key</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>main_page</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>page_params</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>menu_key</td>

<td>varchar(191)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>display_on_menu</td>

<td>char(1)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td>N</td>

<td></td>

<td></td>

</tr>

<tr>

<td>sort_order</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## admin_pages_to_profiles

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**profile_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

**page_key**

</td>

<td>varchar(191)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## admin_profiles

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**profile_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>profile_name</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## authorizenet

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**id**

</td>

<td>int(11) unsigned</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[customer_id](#customers)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[order_id](#orders)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>response_code</td>

<td>int(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>response_text</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>authorization_type</td>

<td>varchar(50)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>transaction_id</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>sent</td>

<td>longtext</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>received</td>

<td>longtext</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>time</td>

<td>varchar(50)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>session_id</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## banners

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**banners_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>banners_title</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>banners_url</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>banners_image</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>banners_group</td>

<td>varchar(15)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>banners_html_text</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>expires_impressions</td>

<td>int(7)</td>

<td></td>

<td>YES</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>expires_date</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_scheduled</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_status_change</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>status</td>

<td>int(1)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>banners_open_new_windows</td>

<td>int(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>banners_on_ssl</td>

<td>int(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>banners_sort_order</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## banners_history

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**banners_history_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[banners_id](#banners)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>banners_shown</td>

<td>int(5)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>banners_clicked</td>

<td>int(5)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>banners_history_date</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## categories

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**categories_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>categories_image</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>parent_id</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>sort_order</td>

<td>int(3)</td>

<td></td>

<td>YES</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>categories_status</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>1</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## categories_description

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**categories_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[language_id](#languages)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>categories_name</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>categories_description</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## configuration

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**configuration_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>configuration_title</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>configuration_key</td>

<td>varchar(180)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>UNI</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>configuration_value</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>configuration_description</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>configuration_group_id</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>sort_order</td>

<td>int(5)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>use_function</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>set_function</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>val_function</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## configuration_group

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**configuration_group_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>configuration_group_title</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>configuration_group_description</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>sort_order</td>

<td>int(5)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>visible</td>

<td>int(1)</td>

<td></td>

<td>YES</td>

<td>MUL</td>

<td>1</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## counter

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>startdate</td>

<td>char(8)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>counter</td>

<td>int(12)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## counter_history

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**startdate**

</td>

<td>char(8)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>counter</td>

<td>int(12)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>session_counter</td>

<td>int(12)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## countries

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**countries_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>countries_name</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>countries_iso_code_2</td>

<td>char(2)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>countries_iso_code_3</td>

<td>char(3)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>address_format_id</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>status</td>

<td>tinyint(1)</td>

<td></td>

<td>YES</td>

<td></td>

<td>1</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## coupon_email_track

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**unique_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[coupon_id](#coupons)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>customer_id_sent</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>sent_firstname</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>sent_lastname</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>emailed_to</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_sent</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## coupon_gv_customer

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**customer_id**

</td>

<td>int(5)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>amount</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## coupon_gv_queue

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**unique_id**

</td>

<td>int(5)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[customer_id](#customers)</td>

<td>int(5)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[order_id](#orders)</td>

<td>int(5)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>amount</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_created</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>ipaddr</td>

<td>varchar(45)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>release_flag</td>

<td>char(1)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td>N</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## coupon_redeem_track

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**unique_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[coupon_id](#coupons)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[customer_id](#customers)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>redeem_date</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>redeem_ip</td>

<td>varchar(45)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[order_id](#orders)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## coupon_restrict

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**restrict_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[coupon_id](#coupons)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[product_id](#products)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[category_id](#categories)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>coupon_restrict</td>

<td>char(1)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td>N</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## coupons

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**coupon_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>coupon_type</td>

<td>char(1)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td>F</td>

<td></td>

<td></td>

</tr>

<tr>

<td>coupon_code</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>coupon_amount</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>coupon_minimum_order</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>coupon_start_date</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>coupon_expire_date</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>uses_per_coupon</td>

<td>int(5)</td>

<td></td>

<td>NO</td>

<td></td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>uses_per_user</td>

<td>int(5)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>restrict_to_products</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>restrict_to_categories</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>restrict_to_customers</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>coupon_active</td>

<td>char(1)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td>Y</td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_created</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_modified</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>coupon_zone_restriction</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>coupon_calc_base</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>coupon_order_limit</td>

<td>int(4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>coupon_is_valid_for_sales</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>coupon_product_count</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## coupons_description

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**coupon_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[language_id](#languages)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>coupon_name</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>coupon_description</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## currencies

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**currencies_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>title</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>code</td>

<td>char(3)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>symbol_left</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>symbol_right</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>decimal_point</td>

<td>char(1)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>thousands_point</td>

<td>char(1)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>decimal_places</td>

<td>char(1)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>value</td>

<td>decimal(14,6)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_updated</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## customers

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**customers_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>customers_gender</td>

<td>char(1)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_firstname</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_lastname</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_dob</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_email_address</td>

<td>varchar(96)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_nick</td>

<td>varchar(96)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[customers_default_address_id](#address_book)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_telephone</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_fax</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_password</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_newsletter</td>

<td>char(1)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[customers_group_pricing](#group_pricing)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_email_format</td>

<td>varchar(4)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td>TEXT</td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_authorization</td>

<td>int(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_referral</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_paypal_payerid</td>

<td>varchar(20)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_paypal_ec</td>

<td>tinyint(1) unsigned</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## customers_basket

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**customers_basket_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[customers_id](#customers)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[products_id](#products)</td>

<td>tinytext</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_basket_quantity</td>

<td>float</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_basket_date_added</td>

<td>varchar(8)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## customers_basket_attributes

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**customers_basket_attributes_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[customers_id](#customers)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[products_id](#products)</td>

<td>tinytext</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[products_options_id](#products_options)</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[products_options_value_id](#products_options_values)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options_value_text</td>

<td>blob</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options_sort_order</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## customers_info

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**customers_info_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_info_date_of_last_logon</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_info_number_of_logons</td>

<td>int(5)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_info_date_account_created</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_info_date_account_last_modified</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>global_product_notifications</td>

<td>int(1)</td>

<td></td>

<td>YES</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## db_cache

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**cache_entry_name**

</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>cache_data</td>

<td>mediumblob</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>cache_entry_created</td>

<td>int(15)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## email_archive

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**archive_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>email_to_name</td>

<td>varchar(96)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>email_to_address</td>

<td>varchar(96)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>email_from_name</td>

<td>varchar(96)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>email_from_address</td>

<td>varchar(96)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>email_subject</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>email_html</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>email_text</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_sent</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>module</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## ezpages

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**pages_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>alt_url</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>alt_url_external</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>status_header</td>

<td>int(1)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>status_sidebox</td>

<td>int(1)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>status_footer</td>

<td>int(1)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>status_visible</td>

<td>int(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>status_toc</td>

<td>int(1)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>header_sort_order</td>

<td>int(3)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>sidebox_sort_order</td>

<td>int(3)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>footer_sort_order</td>

<td>int(3)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>toc_sort_order</td>

<td>int(3)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>page_open_new_window</td>

<td>int(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>page_is_ssl</td>

<td>int(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>toc_chapter</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## ezpages_content

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**pages_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[languages_id](#languages)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>pages_title</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>pages_html_text</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## featured

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**featured_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[products_id](#products)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>featured_date_added</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>featured_last_modified</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>expires_date</td>

<td>date</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0001-01-01</td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_status_change</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>status</td>

<td>int(1)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>featured_date_available</td>

<td>date</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0001-01-01</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## files_uploaded

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**files_uploaded_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>sesskey</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[customers_id](#customers)</td>

<td>int(11)</td>

<td></td>

<td>YES</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>files_uploaded_name</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## geo_zones

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**geo_zone_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>geo_zone_name</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>geo_zone_description</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## get_terms_to_filter

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**get_term_name**

</td>

<td>varchar(191)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>get_term_table</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>get_term_name_field</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## group_pricing

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**group_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>group_name</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>group_percentage</td>

<td>decimal(5,2)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## languages

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**languages_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>name</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>code</td>

<td>char(2)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>image</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>directory</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>sort_order</td>

<td>int(3)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## layout_boxes

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**layout_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>layout_template</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>layout_box_name</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>layout_box_status</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>layout_box_location</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>layout_box_sort_order</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>layout_box_sort_order_single</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>layout_box_status_single</td>

<td>tinyint(4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## manufacturers

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**manufacturers_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>manufacturers_name</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>manufacturers_image</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## manufacturers_info

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**manufacturers_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[languages_id](#languages)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>manufacturers_url</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>url_clicked</td>

<td>int(5)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_last_click</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## media_clips

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**clip_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>media_id</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>clip_type</td>

<td>smallint(6)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>clip_filename</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## media_manager

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**media_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>media_name</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## media_to_products

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>media_id</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[product_id](#products)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## media_types

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**type_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>type_name</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>type_ext</td>

<td>varchar(8)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## meta_tags_categories_description

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**categories_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[language_id](#languages)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>metatags_title</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>metatags_keywords</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>metatags_description</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## meta_tags_products_description

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**products_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[language_id](#languages)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>metatags_title</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>metatags_keywords</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>metatags_description</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## music_genre

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**music_genre_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>music_genre_name</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## newsletters

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**newsletters_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>title</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>content</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>content_html</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>module</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_sent</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>status</td>

<td>int(1)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>locked</td>

<td>int(1)</td>

<td></td>

<td>YES</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## orders

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**orders_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[customers_id](#customers)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_name</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_company</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_street_address</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_suburb</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_city</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_postcode</td>

<td>varchar(10)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_state</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_country</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_telephone</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_email_address</td>

<td>varchar(96)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_address_format_id</td>

<td>int(5)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>delivery_name</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>delivery_company</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>delivery_street_address</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>delivery_suburb</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>delivery_city</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>delivery_postcode</td>

<td>varchar(10)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>delivery_state</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>delivery_country</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>delivery_address_format_id</td>

<td>int(5)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>billing_name</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>billing_company</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>billing_street_address</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>billing_suburb</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>billing_city</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>billing_postcode</td>

<td>varchar(10)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>billing_state</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>billing_country</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>billing_address_format_id</td>

<td>int(5)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>payment_method</td>

<td>varchar(128)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>payment_module_code</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>shipping_method</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>shipping_module_code</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>coupon_code</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>cc_type</td>

<td>varchar(20)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>cc_owner</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>cc_number</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>cc_expires</td>

<td>varchar(4)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>cc_cvv</td>

<td>blob</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_purchased</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>orders_status</td>

<td>int(5)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>orders_date_finished</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>currency</td>

<td>char(3)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>currency_value</td>

<td>decimal(14,6)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>order_total</td>

<td>decimal(15,4)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>order_tax</td>

<td>decimal(15,4)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>paypal_ipn_id</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>ip_address</td>

<td>varchar(96)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>order_weight</td>

<td>float</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## orders_products

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**orders_products_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[orders_id](#orders)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[products_id](#products)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_model</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_name</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_price</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>final_price</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_tax</td>

<td>decimal(7,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_quantity</td>

<td>float</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>onetime_charges</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_priced_by_attribute</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>product_is_free</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_discount_type</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_discount_type_from</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[products_prid](#products)</td>

<td>tinytext</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_weight</td>

<td>float</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_virtual</td>

<td>tinyint(1)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>product_is_always_free_shipping</td>

<td>tinyint(1)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_quantity_order_min</td>

<td>float</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_quantity_order_units</td>

<td>float</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_quantity_order_max</td>

<td>float</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_quantity_mixed</td>

<td>tinyint(1)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_mixed_discount_quantity</td>

<td>tinyint(1)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## orders_products_attributes

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**orders_products_attributes_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[orders_id](#orders)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[orders_products_id](#orders_products)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options_values</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>options_values_price</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>price_prefix</td>

<td>char(1)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>product_attribute_is_free</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_attributes_weight</td>

<td>float</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_attributes_weight_prefix</td>

<td>char(1)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_discounted</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_base_included</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_onetime</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_factor</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_factor_offset</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_factor_onetime</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_factor_onetime_offset</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_qty_prices</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_qty_prices_onetime</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_words</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_words_free</td>

<td>int(4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_letters</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_letters_free</td>

<td>int(4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[products_options_id](#products_options)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options_values_id</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[products_prid](#products)</td>

<td>tinytext</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## orders_products_download

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**orders_products_download_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[orders_id](#orders)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[orders_products_id](#orders_products)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>orders_products_filename</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>download_maxdays</td>

<td>int(2)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>download_count</td>

<td>int(2)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[products_prid](#products)</td>

<td>tinytext</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_attributes_id</td>

<td>int(11)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## orders_status

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**orders_status_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[language_id](#languages)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>orders_status_name</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## orders_status_history

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**orders_status_history_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[orders_id](#orders)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[orders_status_id](#orders_status)</td>

<td>int(5)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>customer_notified</td>

<td>int(1)</td>

<td></td>

<td>YES</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>comments</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>updated_by</td>

<td>varchar(45)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## orders_total

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**orders_total_id**

</td>

<td>int(10) unsigned</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[orders_id](#orders)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>title</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>text</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>value</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>class</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>sort_order</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## paypal

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**paypal_ipn_id**

</td>

<td>int(11) unsigned</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[order_id](#orders)</td>

<td>int(11) unsigned</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>txn_type</td>

<td>varchar(40)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>module_name</td>

<td>varchar(40)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>module_mode</td>

<td>varchar(40)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>reason_code</td>

<td>varchar(40)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>payment_type</td>

<td>varchar(40)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>payment_status</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>pending_reason</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>invoice</td>

<td>varchar(128)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>mc_currency</td>

<td>char(3)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>first_name</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_name</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>payer_business_name</td>

<td>varchar(128)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>address_name</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>address_street</td>

<td>varchar(254)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>address_city</td>

<td>varchar(120)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>address_state</td>

<td>varchar(120)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>address_zip</td>

<td>varchar(10)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>address_country</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>address_status</td>

<td>varchar(11)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>payer_email</td>

<td>varchar(128)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>payer_id</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>payer_status</td>

<td>varchar(10)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>payment_date</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>business</td>

<td>varchar(128)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>receiver_email</td>

<td>varchar(128)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>receiver_id</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>txn_id</td>

<td>varchar(20)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>parent_txn_id</td>

<td>varchar(20)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>num_cart_items</td>

<td>tinyint(4) unsigned</td>

<td></td>

<td>NO</td>

<td></td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>mc_gross</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>mc_fee</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>payment_gross</td>

<td>decimal(15,4)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>payment_fee</td>

<td>decimal(15,4)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>settle_amount</td>

<td>decimal(15,4)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>settle_currency</td>

<td>char(3)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>exchange_rate</td>

<td>decimal(15,4)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>notify_version</td>

<td>varchar(6)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>verify_sign</td>

<td>varchar(128)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>memo</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## paypal_payment_status

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**payment_status_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>payment_status_name</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## paypal_payment_status_history

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**payment_status_history_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>paypal_ipn_id</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>txn_id</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>parent_txn_id</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>payment_status</td>

<td>varchar(17)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>pending_reason</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## paypal_session

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**unique_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>session_id</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>saved_session</td>

<td>mediumblob</td>

<td></td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>expiry</td>

<td>int(17)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## paypal_testing

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**paypal_ipn_id**

</td>

<td>int(11) unsigned</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[order_id](#orders)</td>

<td>int(11) unsigned</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>custom</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>txn_type</td>

<td>varchar(40)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>module_name</td>

<td>varchar(40)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>module_mode</td>

<td>varchar(40)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>reason_code</td>

<td>varchar(40)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>payment_type</td>

<td>varchar(40)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>payment_status</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>pending_reason</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>invoice</td>

<td>varchar(128)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>mc_currency</td>

<td>char(3)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>first_name</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_name</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>payer_business_name</td>

<td>varchar(128)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>address_name</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>address_street</td>

<td>varchar(254)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>address_city</td>

<td>varchar(120)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>address_state</td>

<td>varchar(120)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>address_zip</td>

<td>varchar(10)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>address_country</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>address_status</td>

<td>varchar(11)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>payer_email</td>

<td>varchar(128)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>payer_id</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>payer_status</td>

<td>varchar(10)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>payment_date</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>business</td>

<td>varchar(128)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>receiver_email</td>

<td>varchar(128)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>receiver_id</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>txn_id</td>

<td>varchar(20)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>parent_txn_id</td>

<td>varchar(20)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>num_cart_items</td>

<td>tinyint(4) unsigned</td>

<td></td>

<td>NO</td>

<td></td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>mc_gross</td>

<td>decimal(7,2)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>mc_fee</td>

<td>decimal(7,2)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>payment_gross</td>

<td>decimal(7,2)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>payment_fee</td>

<td>decimal(7,2)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>settle_amount</td>

<td>decimal(7,2)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>settle_currency</td>

<td>char(3)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>exchange_rate</td>

<td>decimal(4,2)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>notify_version</td>

<td>decimal(2,1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>verify_sign</td>

<td>varchar(128)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>memo</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## product_music_extra

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**products_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[artists_id](#record_artists)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>record_company_id</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>music_genre_id</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## product_type_layout

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**configuration_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>configuration_title</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>configuration_key</td>

<td>varchar(180)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>UNI</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>configuration_value</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>configuration_description</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>product_type_id</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>sort_order</td>

<td>int(5)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>use_function</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>set_function</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## product_types

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**type_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>type_name</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>type_handler</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>type_master_type</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>allow_add_to_cart</td>

<td>char(1)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td>Y</td>

<td></td>

<td></td>

</tr>

<tr>

<td>default_image</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## product_types_to_category

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>product_type_id</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[category_id](#categories)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## products

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**products_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>products_type</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_quantity</td>

<td>float</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_model</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_image</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_price</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_virtual</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_date_added</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_last_modified</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_date_available</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_weight</td>

<td>float</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_status</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_tax_class_id</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>manufacturers_id</td>

<td>int(11)</td>

<td></td>

<td>YES</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_ordered</td>

<td>float</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_quantity_order_min</td>

<td>float</td>

<td></td>

<td>NO</td>

<td></td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_quantity_order_units</td>

<td>float</td>

<td></td>

<td>NO</td>

<td></td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_priced_by_attribute</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>product_is_free</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>product_is_call</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_quantity_mixed</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>product_is_always_free_shipping</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_qty_box_status</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_quantity_order_max</td>

<td>float</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_sort_order</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_discount_type</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_discount_type_from</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_price_sorter</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[master_categories_id](#categories)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_mixed_discount_quantity</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>metatags_title_status</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>metatags_products_name_status</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>metatags_model_status</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>metatags_price_status</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>metatags_title_tagline_status</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## products_attributes

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**products_attributes_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[products_id](#products)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[options_id](#products_options)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[options_values_id](#products_options_values)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>options_values_price</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>price_prefix</td>

<td>char(1)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options_sort_order</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>product_attribute_is_free</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_attributes_weight</td>

<td>float</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_attributes_weight_prefix</td>

<td>char(1)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_display_only</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_default</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_discounted</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_image</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_base_included</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_onetime</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_factor</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_factor_offset</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_factor_onetime</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_factor_onetime_offset</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_qty_prices</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_qty_prices_onetime</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_words</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_words_free</td>

<td>int(4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_letters</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_price_letters_free</td>

<td>int(4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>attributes_required</td>

<td>tinyint(1)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## products_attributes_download

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**products_attributes_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_attributes_filename</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_attributes_maxdays</td>

<td>int(2)</td>

<td></td>

<td>YES</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_attributes_maxcount</td>

<td>int(2)</td>

<td></td>

<td>YES</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## products_description

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**products_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[language_id](#languages)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_name</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_description</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_url</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_viewed</td>

<td>int(5)</td>

<td></td>

<td>YES</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## products_discount_quantity

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>discount_id</td>

<td>int(4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[products_id](#products)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>discount_qty</td>

<td>float</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>discount_price</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## products_notifications

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**products_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[customers_id](#customers)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## products_options

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**products_options_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[language_id](#languages)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options_name</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options_sort_order</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options_type</td>

<td>int(5)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options_length</td>

<td>smallint(2)</td>

<td></td>

<td>NO</td>

<td></td>

<td>32</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options_comment</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options_size</td>

<td>smallint(2)</td>

<td></td>

<td>NO</td>

<td></td>

<td>32</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options_images_per_row</td>

<td>int(2)</td>

<td></td>

<td>YES</td>

<td></td>

<td>5</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options_images_style</td>

<td>int(1)</td>

<td></td>

<td>YES</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options_rows</td>

<td>smallint(2)</td>

<td></td>

<td>NO</td>

<td></td>

<td>1</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## products_options_types

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**products_options_types_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options_types_name</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## products_options_values

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**products_options_values_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[language_id](#languages)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options_values_name</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options_values_sort_order</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## products_options_values_to_products_options

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**products_options_values_to_products_options_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[products_options_id](#products_options)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>products_options_values_id</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## products_to_categories

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**products_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[categories_id](#categories)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## project_version

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**project_version_id**

</td>

<td>tinyint(3)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>project_version_key</td>

<td>varchar(40)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>UNI</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>project_version_major</td>

<td>varchar(20)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>project_version_minor</td>

<td>varchar(20)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>project_version_patch1</td>

<td>varchar(20)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>project_version_patch2</td>

<td>varchar(20)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>project_version_patch1_source</td>

<td>varchar(20)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>project_version_patch2_source</td>

<td>varchar(20)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>project_version_comment</td>

<td>varchar(250)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>project_version_date_applied</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 01:01:01</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## project_version_history

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**project_version_id**

</td>

<td>tinyint(3)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>project_version_key</td>

<td>varchar(40)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>project_version_major</td>

<td>varchar(20)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>project_version_minor</td>

<td>varchar(20)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>project_version_patch</td>

<td>varchar(20)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>project_version_comment</td>

<td>varchar(250)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>project_version_date_applied</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 01:01:01</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## query_builder

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**query_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>query_category</td>

<td>varchar(40)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>query_name</td>

<td>varchar(80)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>UNI</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>query_description</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>query_string</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>query_keys_list</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## record_artists

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**artists_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>artists_name</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>artists_image</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## record_artists_info

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**artists_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[languages_id](#languages)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>artists_url</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>url_clicked</td>

<td>int(5)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_last_click</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## record_company

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**record_company_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>record_company_name</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>record_company_image</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## record_company_info

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**record_company_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[languages_id](#languages)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>record_company_url</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>url_clicked</td>

<td>int(5)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_last_click</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## reviews

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**reviews_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[products_id](#products)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[customers_id](#customers)</td>

<td>int(11)</td>

<td></td>

<td>YES</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>customers_name</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>reviews_rating</td>

<td>int(1)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>reviews_read</td>

<td>int(5)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>status</td>

<td>int(1)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>1</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## reviews_description

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**reviews_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[languages_id](#languages)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>reviews_text</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## salemaker_sales

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**sale_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>sale_status</td>

<td>tinyint(4)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>sale_name</td>

<td>varchar(128)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>sale_deduction_value</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>sale_deduction_type</td>

<td>tinyint(4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>sale_pricerange_from</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>sale_pricerange_to</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>sale_specials_condition</td>

<td>tinyint(4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>sale_categories_selected</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>sale_categories_all</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>sale_date_start</td>

<td>date</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0001-01-01</td>

<td></td>

<td></td>

</tr>

<tr>

<td>sale_date_end</td>

<td>date</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0001-01-01</td>

<td></td>

<td></td>

</tr>

<tr>

<td>sale_date_added</td>

<td>date</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01</td>

<td></td>

<td></td>

</tr>

<tr>

<td>sale_date_last_modified</td>

<td>date</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01</td>

<td></td>

<td></td>

</tr>

<tr>

<td>sale_date_status_change</td>

<td>date</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## sessions

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**sesskey**

</td>

<td>varchar(191)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>expiry</td>

<td>int(11) unsigned</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>value</td>

<td>mediumblob</td>

<td></td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## specials

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**specials_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[products_id](#products)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>specials_new_products_price</td>

<td>decimal(15,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>specials_date_added</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>specials_last_modified</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>expires_date</td>

<td>date</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0001-01-01</td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_status_change</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>status</td>

<td>int(1)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>specials_date_available</td>

<td>date</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0001-01-01</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## tax_class

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**tax_class_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>tax_class_title</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>tax_class_description</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## tax_rates

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**tax_rates_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>tax_zone_id</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[tax_class_id](#tax_class)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>tax_priority</td>

<td>int(5)</td>

<td></td>

<td>YES</td>

<td></td>

<td>1</td>

<td></td>

<td></td>

</tr>

<tr>

<td>tax_rate</td>

<td>decimal(7,4)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0.0000</td>

<td></td>

<td></td>

</tr>

<tr>

<td>tax_description</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## template_select

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**template_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>template_dir</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>template_language</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## upgrade_exceptions

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**upgrade_exception_id**

</td>

<td>smallint(5)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>sql_file</td>

<td>varchar(128)</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>reason</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>errordate</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>sqlstatement</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## whos_online

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>customer_id</td>

<td>int(11)</td>

<td></td>

<td>YES</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>full_name</td>

<td>varchar(64)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>session_id</td>

<td>varchar(191)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>ip_address</td>

<td>varchar(45)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>time_entry</td>

<td>varchar(14)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>time_last_click</td>

<td>varchar(14)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_page_url</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>host_address</td>

<td>text</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>user_agent</td>

<td>varchar(255)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## zones

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**zone_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[zone_country_id](#countries)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>MUL</td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>zone_code</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>zone_name</td>

<td>varchar(32)</td>

<td>utf8mb4_general_ci</td>

<td>NO</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

## zones_to_geo_zones

<table>

<tbody>

<tr>

<td>Field</td>

<td>Type</td>

<td>Collation</td>

<td>Null</td>

<td>Key</td>

<td>Default</td>

<td>Extra</td>

<td>Comment</td>

</tr>

<tr>

<td>

**association_id**

</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td>PRI</td>

<td></td>

<td>auto_increment</td>

<td></td>

</tr>

<tr>

<td>

[zone_country_id](#countries)</td>

<td>int(11)</td>

<td></td>

<td>NO</td>

<td></td>

<td>0</td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[zone_id](#zones)</td>

<td>int(11)</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>

[geo_zone_id](#geo_zones)</td>

<td>int(11)</td>

<td></td>

<td>YES</td>

<td>MUL</td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>last_modified</td>

<td>datetime</td>

<td></td>

<td>YES</td>

<td></td>

<td></td>

<td></td>

<td></td>

</tr>

<tr>

<td>date_added</td>

<td>datetime</td>

<td></td>

<td>NO</td>

<td></td>

<td>0001-01-01 00:00:00</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

