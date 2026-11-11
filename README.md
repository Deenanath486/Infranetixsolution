# INFRANETIX SOLUTIONS

INFRANETIX SOLUTIONS ke liye ek responsive static website. Is project mein home broadband, dedicated leased line, enterprise internet, service enquiry, support aur admin enquiry-management pages included hain.

## Pages

- `index.html` - Homepage aur services overview
- `broadband.html` - Home broadband plans
- `leased-line.html` - Dedicated leased line solutions
- `enterprise.html` - Enterprise connectivity services
- `about.html` - Company information
- `contact.html` - Contact details aur enquiry form
- `support.html` - Customer support aur chatbot
- `quote.html` - Custom quotation request form
- `404.html` - Custom not-found page
- `admin/index.html` - Admin login
- `admin/dashboard.html` - Enquiry management dashboard

## Features

- Fully responsive desktop aur mobile layout
- Mobile navigation menu
- Scroll animations aur interactive speed counter
- Service-specific content pages
- Quote aur contact enquiry forms
- Interactive support chatbot
- Browser-based admin dashboard
- Enquiry search, status management, customer view aur CSV export
- Browser `localStorage` mein enquiry data
- Admin session browser `sessionStorage` mein manage hoti hai

## Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- Font Awesome 6
- Google Fonts

Koi build process ya backend dependency nahi hai.

## Local Setup

Repository ko clone/open karne ke baad project folder ke andar terminal open karein.

### Python se run karein

```bash
python -m http.server 8000
```

Phir browser mein `http://localhost:8000` open karein.

### VS Code Live Server se run karein

1. `Live Server` extension install karein.
2. `index.html` par right-click karein.
3. **Open with Live Server** select karein.

## Admin Dashboard

Admin login:

```text
URL: /admin/
Username: admin
Password: infranetix@2024
```

> Demo configuration: Source code mein credentials present hain, isliye hosting se pehle credentials change aur proper server-side authentication implement karni chahiye. Frontend admin login aur session check production security ke liye suitable nahi hain.

## Data Storage

Quote enquiries browser ke `localStorage` mein `infranetix_enquiries` key ke andar store hoti hain. Admin dashboard isi data ko read, update, filter aur CSV format mein export karta hai.

Local browser data ko test karne ke liye:

```javascript
localStorage.getItem("infranetix_enquiries");
```

## Deployment

Website ko kisi bhi static hosting service par deploy kiya ja sakta hai, jaise:

- GitHub Pages
- Netlify
- Vercel
- Cloudflare Pages
- Traditional shared hosting

Deploy karte waqt project ke saare files same relative structure mein upload karein. External Font Awesome aur Google Fonts resources internet access par depend karte hain.

## Project Structure

```text
.
|-- index.html
|-- broadband.html
|-- leased-line.html
|-- enterprise.html
|-- about.html
|-- contact.html
|-- support.html
|-- quote.html
|-- 404.html
|-- robots.txt
|-- sitemap.xml
|-- admin/
|   |-- index.html
|   `-- dashboard.html
`-- assets/
    |-- css/
    |   `-- style.css
    |-- js/
    |   |-- main.js
    |   `-- chatbot.js
    `-- images/
```
