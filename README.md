# Navitru — Smart Hospital Navigation System

Navitru is a browser-based hospital navigation interface designed to help patients and visitors find departments, doctors, cabins, and rooms, and access appointment-related information.

## Features

- **Patient workflow:** Enter a receipt/token number or use department, sub-department, and doctor selection.
- **Hospital navigation:** Opens an embedded indoor-navigation view.
- **Doctor and appointment information:** Displays available appointment-related details and queue estimates when the required data is available.
- **Voice input:** Supports speech-based receipt/token entry in compatible browsers, with a confirmation step.
- **English/Hindi interface:** Includes language-aware interface text.
- **Patient utilities:** Includes entry points for medicine reminders, visit history, and missed appointments.
- **Admin entry point:** Provides an admin workflow entry. The HTML file indicates that the separate `admin.html` portal is expected when running in live/server mode.
- **Responsive UI:** Layouts are designed for desktop and mobile screens.
- **Homepage AI chatbot:** The AI chatbot/agent shown on the home page was created using **Agent37**. It helps users with common questions about using Navitru.
- **Help assistant:** Includes a built-in assistant for common questions about using Navitru.

## Project type

This version is a **single-page HTML application**. Its markup, CSS styles, and JavaScript are bundled into one HTML file.

## Files

- `navitru_final_chatbot.html` — main Navitru application.

Depending on how the live deployment is configured, additional server-side files may be needed, including `admin.html`, hospital data/API services, and the indoor-navigation page loaded by the application. Those files are not included in this single HTML file.

## External resources

The HTML references external resources, including:

- Google Fonts (`Poppins` and `Atkinson Hyperlegible`)
- Lucide icons via the `unpkg.com` CDN

An internet connection may be needed for these external resources to load. Browser speech-recognition support also varies by browser and platform.

## Important notes and limitations

- **Local/demo mode is not the same as a live hospital deployment.** The code includes logic that distinguishes live mode from a standalone copy. Some features may need the hospital server or additional files to work fully.
- **Admin portal:** In live mode, the app navigates to `admin.html`; that separate page is not part of this HTML file.
- **Data and queue estimates:** Accuracy depends on the hospital data and the data/API source actually connected to the application. Do not treat demo or sample queue estimates as real-time clinical or operational information.
- **Indoor navigation:** The navigation screen embeds another page in an iframe. That destination must be available and correctly configured for directions to work.
- **Browser storage:** Some preferences, such as language, are stored locally in the browser.
- **Privacy:** Before using this with real patients, review data storage, access controls, authentication, and privacy/security requirements. Do not put real patient data into a public demo.

## Suggested next steps for deployment

1. Provide and configure the hospital's authoritative department, doctor, cabin, room, and appointment data.
2. Connect queue estimates to a maintained source of real appointment/queue data.
3. Configure and test the indoor-navigation page and its iframe integration.
4. Deploy the admin portal separately with server-side authentication and authorization.
5. Test voice input, language selection, navigation, and responsive layouts on target devices.
6. Review accessibility, privacy, and security before production use.

## Technology

- HTML
- CSS
- JavaScript
- Google Fonts
- Lucide icons
- **Agent37** for the home-page AI chatbot agent
- Browser speech-recognition APIs where supported

## License

No license is specified in the provided HTML file. Add a `LICENSE` file if you intend to publish or distribute the project, and make sure any third-party assets are used in accordance with their licenses.
