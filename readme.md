# Angular Weather App

A simple weather app built using Angular. It shows real-time weather data from a weather API.

---

## Prerequisites

Install the following before you begin:

- Node.js (v16 recommended)
- npm (comes with Node.js)
- Angular CLI
- Git

If you're using Node.js v17 or higher, you must set an extra flag due to crypto module issues. See Step 4.

---

## How to Run the App

Follow these steps to set up and run the project:

---

### Step 1: Clone the Repository

```bash
git clone https://github.com/Karthick-MurugesanG/Angular_Weather_app.git
cd AngularWeatherApp
```


---

### Step 2: Install Angular CLI (if not already installed)

```bash
npm install -g @angular/cli
```

---

### Step 3: Install Dependencies

```bash
npm install
```

This installs all required packages listed in `package.json`.

---

### Step 4: Fix for Node.js v17+ (only if needed)

If you're using Node.js v17 or newer, set the legacy OpenSSL flag before running:

**Windows CMD:**

```bash
set NODE_OPTIONS=--openssl-legacy-provider
```

**PowerShell:**

```powershell
$env:NODE_OPTIONS="--openssl-legacy-provider"
```

**macOS/Linux:**

```bash
export NODE_OPTIONS=--openssl-legacy-provider
```

---

### Step 5: Serve the Application

```bash
ng serve
```

Then open your browser and visit:

```
http://localhost:4200/
```

---

## Build for Production

```bash
ng build
```

The production-ready files will be in the `dist/` folder.

---

## Project Structure

```
AngularWeatherApp/
├── src/
│   ├── app/
│   ├── assets/
│   └── environments/
├── angular.json
├── package.json
├── tsconfig.json
└── README.md
```

---

## Common Issues

- `ng: command not found` → Install Angular CLI globally using `npm install -g @angular/cli`
- `crypto error / openssl error` → Set `NODE_OPTIONS` as shown in Step 4

---

## License

MIT License
