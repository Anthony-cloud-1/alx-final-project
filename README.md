# Overview

This is a cyber bullying detection system integrated with Google's `GEMINNI AI`

## Setup Instructions

### 1. Clone the Repository

First, clone the repository to your local machine:

```bash
git clone <repository-url>
cd <repository-directory>
```

### 2. Install Dependencies

Install the required Node.js packages using npm in each of the directories:

```bash
npm install
```

### 3. Create Environment Configuration File

Create a `.env` file in the `CyberWatchGemini` directory of the project. This file will contain all the necessary environment variables. Use the following template and fill in the required values:

```dotenv
GOOGLE_GENAI_API_KEY=XXXXXXXXXXXXXXXXXXXXXXXXXXXXX
```

## 4. Developing

Once you've installed the dependencies with `npm install` (or `pnpm install` or `yarn`) in both directories, start a development server in the `CyberWatch` directory:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## 5. Developing

Start the `AI` in the `CyberWatchGemini/lib` directory:

```bash
node index.js
```
