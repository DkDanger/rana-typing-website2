# RANA TYPING website

This is a static, responsive recreation of the Pomelli website at `https://labs.google.com/pomelli/website/9dnpr_CeJ5M9U7PCyj4O76`. It includes the visible page sections, service descriptions, location/contact details, the supplied Paytm QR image, and the service photographs from the Pomelli page.

A dedicated CSC Services section now includes 12 cards: Aadhaar, PAN, banking/BC, insurance, government schemes and forms, bill payments, recharge, education, online applications, printing/scanning, and digital documentation. These cards use the same bilingual details popups and carousel controls as the other service groups. Photo source links and license notes are in `assets/SOURCES.txt`. The page also has eight more contact cards for advocate connections, certified-copy help, web design, website building, Android apps, custom lithium batteries, electrician contacts, and carpenter contacts.

## Files

- `index.html` — page structure and business content
- `styles.css` — responsive styling
- `script.js` — Hindi/English switch, mobile menu, service detail popups, and website search
- `assets/` — all page images, QR image, and favicon

## Notes before publishing

- This website has its own separate Counter Gratis ID (`b96633eb`); it does not share its total with `www.ranatyping.co.in`. The provider counts one visitor per IP address per UTC day, so it measures daily unique IPs rather than identifying a person permanently. The live counter works after the page is hosted online and needs an internet connection.
- All three service-card rows move slowly and continuously by default; each row travels in the direction opposite to its neighboring row. Visitors can pause them briefly with the arrows, swipe or scroll them, or use the keyboard. The motion respects reduced-motion settings.
- The Store button opens `https://tradoi.com/store/rana-typing-hazaribagh` in a new tab.
- The reservation buttons point to `ranatyping.co.in`, as shown on the source page. Update this URL if you want a different booking destination.
- The page loads Google Fonts and Material Icons from Google, so those typefaces/icons need an internet connection. The photographs and QR image are included locally in `assets/`.
- Check the payment QR on the final domain with a second phone. Confirm the recipient and amount shown by the UPI app before accepting payments.

## Acts and Sections PDF library

- The header button opens a bilingual Acts and Sections library with the supplied BNS, BNSS, BSA, and IPC PDFs.
- `assets/acts/` contains all eight original Hindi and English PDFs. Keep this folder when uploading the site; the PDFs add about 146 MB to the repository.
- `assets/act-reader.js` and `assets/pdfjs/` provide the in-page PDF reader. Changing the site language switches to the paired PDF and keeps the same page and approximate vertical reading position. The Hindi and English editions have different page counts, so an exact matching line cannot always be guaranteed.
- When opening `index.html` as a `file://` URL, browser security prevents the in-page PDF library from loading. The Act link instead opens the PDF in the browser's built-in reader. GitHub Pages or a local HTTP server enables the in-page reader and synchronized language switch.
- PDF.js is included under its Apache 2.0 license in `assets/pdfjs/LICENSE`.

## Website and PDF search

- The Search button finds matching service and page text. If an Act is open in the in-page reader, it also searches that PDF and lets visitors jump to a matching page.
- Open this site through GitHub Pages or a local HTTP server to search PDFs. A `file://` page can still search the website text, but browser security prevents the in-page reader from loading the PDF search engine.
- PDF search reads selectable text. Scanned page images without text recognition cannot be searched.
- The official Hazaribag Court and district website links are in the legal-service cards. The other contact buttons open WhatsApp with a service-specific message.
## Upload to GitHub Pages

1. Create a GitHub repository and upload the contents of this folder into the repository root. Include the `assets` folder.
2. Open **Settings → Pages** in the repository.
3. Choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
4. When GitHub shows the Pages URL, open it and review the page.
5. For a custom domain, enter the domain in **Settings → Pages → Custom domain**, then add the DNS records GitHub shows at your domain provider. Enable HTTPS after the DNS check completes.

The original Pomelli site is not exported source code; this package recreates the visible design and content as independent HTML, CSS, JavaScript, and local image files.
