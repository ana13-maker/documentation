---
title: Shipping Problems 
category: troubleshooting
weight: 1
---

### My shipping is figured wrong, it is 3 pounds too heavy
Any shipping module that uses weight for the calculations also takes into account a built-in Tare weight.
The Tare setting (configurable in your store Admin) adds extra weight to compensate for packaging materials.

To change the Tare point your cursor at the Configuration menu, choose Shipping/Packaging from the menu and change the Tare.

You can set either and/or both a percentage or weight for Tare and Large Package.

Entered as percentage:weight

**Examples:**
```
Disabled completely = 0:0
10% + 1lb = 10:1
0% +3lb = 0:3
5% + 0lbs = 5:0
```

This way both the Tare for small to medium packages has a flexible option of percentage + weight and the Large Package increase has an option of a percentage + weight.
<hr />

### Sorry, we are not shipping to your region at this time.
This message usually occurs when you have no available shipping modules for that customer's address.

A module is unavailable for one of two reasons:
it's not installed
or it's installed but has a Shipping Zone restriction set on it, and the customer's shipping address isn't in that specified zone.


Or maybe the order qualifies for Free Shipping, but you don't have the freeshipper module installed.

<hr />

### The USPS module is returning an error when I try to checkout

If you are recieving this error:

```
An error occured with the USPS shipping calculations. If you prefer to use USPS as your shipping method, please contact the store owner.
```

You need to call or email USPS and have them move your account to the production server.

See [USPS Setup](/user/modules/usps_setup/).

<hr />
