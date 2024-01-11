# First Milestone Project

# Country Hotel

![Country Hotel log](assets/images/logo.png)

## Table of Contents

- [First Milestone Project](#first-milestone-project)
- [Country Hotel](#country-hotel)
  - [Table of Contents](#table-of-contents)
- [About](#about)
  - [User Experiance (UX)](#user-experiance-ux)
    - [User Stories](#user-stories)
      - [Hotel Owner Goals](#hotel-owner-goals)
      - [Site Visitor Goals](#site-visitor-goals)
- [Design](#design)
    - [Color Scheme](#color-scheme)

# About

Country Hotel is a fictional, family run hotel company. The company owns a hotel in the heart of the British countryside. As a small family run business, the publicity of the company had been only via other media outlets, social media, local phone books and the like. The family have decided, to expand the business, by creating their own website to publicise and promote their hot and services. The decision was to create their own front-end website.

## User Experiance (UX)

### User Stories

#### Hotel Owner Goals

- we want the website to attract a new and wide range of customers.
- We want an attractive website which clearly shows our goals as hotel owners, providing an exclusive experiance to our guests.
- We want the website to be easy and clear to use.
- we want the website to be responsive to all devices.

#### Site Visitor Goals

- I want to have access to clear details regarding the Hotel, if I was to book a stay.
- I want to be able to contact the hotel in the simplest way.
- I want to see what the company have to offer, on their restuarant menu.
- I want the site to be responsive to my device.
- I want the site to be easy to navigate.

# Design

### Color Scheme

I designed my color scheme, based on the Country Hotel logo. For the logo design I used the website Canva (I will isert link to Canva in credits section below). Based on the color of the logo I have designed the website.

- I have used `#425B58` for the dark text in the light background sections of the web pages.
- I have used `#E7D49E` for the light text in the dark background sections of the web pages.
- I have used `#E7D49E` for the light background small sections of the web pages.
- I have used `#425B58` for the dark background sections of the web pages.
- I have used `#FAFADD` for the light background large sections of the web pages.
- I have used `#425B58` for the opaque overlay of bright images.
- I have used `#425B58` for the dark borders.
- I have used `#E7D49E` for the light borders.
- I have used `#927242` for the darker brown text.
- I have used `#2E3F3D` for the darker footer background.
- I have used `#FFFFFF` for the main body background.

![Country Hotel Color Scheme](assets/images/colors.jpg)

### Typography

The fonts used in this website are KoHo and Questrial, both these fonts were sugested for the logo by canva. These fonts work well together where the headers are all KoHo uppercase and the rest of the text across the enrtire website is Questrial.
Both fonts are imported from google fonts asn are used via th import link at the gead of the stylesheet style.css, this links all the text across the pages of the website to the appropriate style annd font.

## Bugs

| No | Bug | How I fixe the bug |
| 1 | The active class on the nav section was a border-bottom solid line, the line was not semetrical below each of nav elements. | I changed the active class, by giving each list item a darker background colour, than the nav bar. |
| 2 | The drop down elements in the navbar, did not dispaly properly on mobile and tablet, the information was blocked by the next list item. | After trying out a few things I realised the dropdown information was only blocked by the second dropdown link, I then changed the order of the nav links. |
| 3 | After I changed the order of the nav links the semetry of the whole nav bar looked odd on desktop | I decided to create two nav links for resturant.html one after both dropdown links for desktop, using the .d bootstrap class I made this one visible only for desktop. The second restaurant.html I placed between the dropdown links and using the .d bootstrap class made it visible only for mobile and tablet. |
| 4 | On restaurant.html I used bootstraps row and col classes to create the information article, the chef info in one column and the genaral info in a second column. After I finished the styling of the chef info and strated with the general info, it came out below the chef info even on desktop. | I spent long time checknig my code to see if I had made mistakes, I compare them to the bootstrap documentation and I could not find the reason for the bug. I tested the link to bootstrap it was working. I then used Devtools and checked multiple times, I relised eventually that the class chef-about which styles the chef info paragraph, I had inserted into the main div of the column (together with the bootstrap class). The chef-about class creates a box whoch is smaller than the overall column width, this therefore caused the next column to start at the edge of the column which was below the chef info. I fixed the bug by creating a separate div for the chef-about class, the main column therefore, used the full width of the page. this gave the space for the next column to start beside the first, rather than under it. |