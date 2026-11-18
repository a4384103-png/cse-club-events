CSE Events Hub
A campus event portal for the Department of Computer Science and Engineering at Rajeev Institute of Technology (RIT), Hassan, organized in collaboration with GDG on Campus – RIT Hassan.

The portal brings technical, cultural, and sports activities into one place. Students can explore events, register individually or in teams, view event scores, and contact coordinators. Coordinators can manage event information through an admin area.
Features
- Home and About: Introduction to the CSE department and GDG on Campus.
- Events: Browse technical, cultural, and sports events. Filter by category and search by event, venue, or coordinator.
- Live Scores: View match/event results and the CSE semester points table.
- Gallery: Browse campus event highlights by category.
- Registration: Register as a solo participant or as a team (2–4 members).
- Student accounts: Sign in or create a student account to access registration features.
- Appointments and inquiries: Request a coordinator appointment or send a message.
- Admin console: Manage registrations, appointments, match scores, points standings, and announcements.
- Theme and responsive navigation: Light/dark theme toggle and mobile navigation.
- Data storage: The page references Supabase for database operations and browser storage as a fallback.
Event categories
1. Technical
2. Cultural
3. Sports
Important: The supplied HTML contains sample/demo event listings, scores, gallery entries, and registration examples. Replace these with verified campus information before using the site for official registrations or announcements.

Technology
The supplied page references the following technologies/assets:
- HTML5
- CSS (external stylesheet)
- JavaScript (external application scripts)
- Supabase JavaScript client / Supabase backend
- Browser storage fallback
The HTML file references these local files in the CSE Events Hub _ Dept. of CSE – RIT Hassan & GDG on Campus_files/ folder:
- supabase.js.download
- main.js.download
- index-CrE-rE_d.css
- Image and font assets
These supporting files are required for the page to work as intended. The HTML file by itself is not a complete project bundle.
Project structure
Keep the HTML file and its companion assets folder together:
CSE-Events-Hub/
├── index.html
└── CSE Events Hub _ Dept. of CSE – RIT Hassan & GDG on Campus_files/
    ├── supabase.js.download
    ├── main.js.download
    ├── index-CrE-rE_d.css
    └── ...images and other assets
You may rename the HTML file to index.html, but do not rename or move the companion assets folder unless you also update the paths in the HTML.
Run locally
1. Download or clone the complete project folder.
2. Make sure index.html and the companion _files folder are in the same directory.
3. Confirm that the JavaScript, CSS, logo, and gallery files referenced by the HTML are present.
4. Open index.html in a modern browser.
For development, you can serve the folder with a local static web server instead of opening the file directly. For example, with Python installed:
python -m http.server 8000
Then open http://localhost:8000 in your browser.
Supabase configuration
The supplied HTML indicates that the application uses Supabase. The actual connection logic is in the referenced JavaScript files, not fully contained in the HTML.

Before deployment:
1. Open the Supabase project and review the required tables and authentication configuration.
2. Configure the project URL and public anon/publishable key in the application JavaScript using your own project settings.
3. Create and verify the database tables, access policies (Row Level Security), and authentication flows required by the application.
4. Never put a Supabase service_role key or other secret credentials in browser-side code.
5. Review the admin authorization rules. Hiding an admin page in the UI is not a security control; enforce permissions in Supabase policies or a trusted server.
6. Test registration, appointment booking, score updates, exports, and offline fallback before publishing.
Do not commit passwords, private keys, or real student personal information to a public repository.
Before publishing
- Replace all sample event, score, gallery, and registration data.
- Verify event dates, venues, coordinator contacts, and participation rules.
- Remove demo credentials and test accounts.
- Add the complete supporting asset files.
- Configure and test Supabase authentication, database policies, and backups.
- Test the site on desktop and mobile browsers.
- Publish only after the department/coordinators approve the content.
Project purpose
CSE Events Hub is intended to provide a single, convenient place for RIT Hassan CSE students to discover campus activities, participate in events, follow results, and communicate with event coordinators.
Credits
Department of Computer Science and Engineering
Rajeev Institute of Technology, Hassan
In collaboration with GDG on Campus – RIT Hassan
