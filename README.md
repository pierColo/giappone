# Japan trip planner

Local trip planner based on `giappone.html`, preserving its visual style and itinerary.

Each day now has a responsive timeline with optional time, cost, Maps location, and booking link. Lunch, dinner, and aperitivo use distinct colored tags. Timed activities sort chronologically; untimed activities retain their position and can be moved with arrows. Legacy backups and existing browser data migrate automatically. The calendar is the initial view and retains its month grid on phones; selecting a day opens its timeline detail.

## Run locally

Requires Node.js. No dependency installation is needed.

```sh
npm run dev
```

Open http://localhost:3000. Edit `index.html` and refresh to see changes.

Run `npm run check` while the local server is running to verify migration, rendering, ordering, backup roundtrips, and the HTTP preview. This check does not replace visual browser QA.

Edits to the itinerary currently save in the browser's local storage. The original HTML and JSON export, import, and print features remain available. Changes previously saved while opening the Downloads file are separate from localhost; export a JSON backup from that file and import it here if needed.

## Next phase

After the requested design and functionality changes, connect Firebase Hosting, Authentication, and Firestore for invitation-based access and shared editing. Firebase is not configured yet.
