# Wedding Seating Lookup App

A simple, elegant web application that allows wedding guests to search for their names and find their assigned table numbers. Built as a single-page static site, perfect for deployment on **GitHub Pages**.

---

## ✨ Features

* **Search by name**: Guests can type their first or last name to find their table.
* **Fuzzy matching**: Handles partial matches, different cases, and accents.
* **CSV-driven**: Reads from a `guests.csv` file in the repo root.
* **Lightweight**: Pure HTML, CSS, and JavaScript—no server required.
* **Guest-facing**: Clean interface with no admin buttons or configuration exposed.

---

## 📂 Repository Structure

```
NIRFAN-Reception-Seating-Chart/
├── index.html     # The main app (this file is deployed via GitHub Pages)
├── guests.csv     # Guest list (Name,Table)
└── README.md      # Project documentation
```

---

## 📝 CSV Format

The application expects a CSV file in the following format:

```csv
Name,Table
John Doe,Table 22
Abel Tesfaye,Table 5
Taylor Swift,Table 18
```

* First row is a header row (`Name,Table`).
* Table values can be in formats like `22`, `Table 22`, or `table22`. The app will normalize to `Table 22`.
* Place `guests.csv` in the **root of the repository**.

---

## 🚀 Deployment

1. Push `index.html` and `guests.csv` to your repo (e.g., `NIRFAN-Reception-Seating-Chart`).
2. In GitHub, go to:

   * **Settings → Pages**
   * Under **Build and deployment → Source**, choose **Deploy from a branch**
   * Branch: `main`, Folder: `/ (root)`
3. Your app will be available at:

   ```
   https://<username>.github.io/NIRFAN-Reception-Seating-Chart/
   ```

---

## 📱 Usage

1. Open the web app link.
2. Enter your full or partial name in the search bar.
3. View your assigned table.

---

## 🎨 Customization

* **Styling**: Adjust colors and fonts in the `<style>` section of `index.html`.
* **Branding**: Add a logo or wedding date inside the `.card` section.
* **QR Code**: Generate a QR code pointing to your GitHub Pages URL and print it on signage for guests.

---

## 🤝 Credits

Developed for **Nirja & Irfan's Reception** 💍
