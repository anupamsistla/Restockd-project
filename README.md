# 🍎 Restockd: Community Food Bank Donation Platform

A full-stack web application that streamlines the coordination between food donors and food banks in real-time. Restock enables food banks to post donation needs, donors to discover nearby opportunities, and both parties to schedule seamless pickups and drop-offs.

**Deployed Website:** [https://restockd-ten.vercel.app](https://restockd-ten.vercel.app)

---

## Key Features

### For Donors
- **Browse & Search** - Discover food banks and their current donation needs using intuitive search filters
- **Schedule Donations** - Book specific times to drop off donations with calendar integration
- **Leaderboard Tracking** - Earn points and see your impact compared to other community members
- **Flexible Scheduling** - Request time changes if your plans shift, with instant food bank notifications

### For Food Banks
- **Post Donation Needs** - Create urgent donation requests with specific items, quantities, and timeframes
- **Manage Donors** - View all scheduled pickups and donor information in one dashboard
- **Coordinate Logistics** - Request time changes from donors when needed
- **Track Donations** - Mark pickups as completed and monitor donation fulfillment
- **Smart Urgency Levels** - Set urgency (Low/Medium/High) to prioritize critical needs

---

## Main Functionality Walkthrough

### User Registration & Login

1. Visit the app and click **Register**
2. Choose your role: **Donor** or **Food Bank**
3. Fill in your information
4. Log in with your credentials

### Donor Workflow

1. **Browse Food Banks** - View all active food banks and their current needs
2. **Search Donations** - Find specific items (e.g., "canned vegetables", "pasta")
3. **Schedule a Pickup** - Click on a donation posting and book a time
4. **Confirm Meetup** - View your scheduled donations in "My Donations"
5. **Track Progress** - Check the Leaderboard to see your donation impact

### Food Bank Workflow

1. **Create Donation Request** - Post what items you need, quantities, and urgency
2. **Manage Donors** - View all donors who have scheduled pickups
3. **Request Time Changes** - If needed, ask donors to reschedule
4. **Mark as Completed** - Confirm when donations are received
5. **View Meetups** - Track all past and upcoming donations in "My Meetups"

---

## 📹 Demo Video

**Watch the full demo:** [View Demo on Google Drive](https://drive.google.com/file/d/1C37JNS-75E3BGBSy8QydT31FMlFyLTu4/view?usp=sharing)

---

## Running the Project Locally

### Clone the Repository

```bash
git clone git@github.com:anupamsistla/Restockd-project.git
cd Restockd
```

### Set Up the Backend (Flask)

Navigate to the backend directory:

```bash
cd backend
```

**Create a virtual environment:**

```bash
# On macOS/Linux
python3 -m venv venv
source venv/bin/activate

# On Windows
python -m venv venv
venv\Scripts\activate
```

**Install dependencies:**

```bash
pip install -r requirements.txt
```

**Set up environment variables:**

Create a `.env` file in the `backend/` directory:

```env
# Supabase Database URL
# Get from: Supabase Dashboard → Settings → Database → Connection string
DATABASE_URL=postgresql://postgres:YOUR_PASSWORD@HOST:5432/postgres

# Flask Configuration
FLASK_ENV=development
FLASK_DEBUG=True
```

**Start the backend server:**

```bash
python app.py
```

---

### Set Up the Frontend (React)

In a new terminal, navigate to the frontend directory:

```bash
cd frontend
```

**Install dependencies:**

```bash
npm install
```

**Set up environment variables:**

Create a `.env.local` file in the `frontend/` directory:

```env
# Supabase Configuration
# Get from: Supabase Dashboard → Settings → API
VITE_SUPABASE_URL=https://YOUR_PROJECT.supabase.co
VITE_SUPABASE_ANON_KEY=YOUR_ANON_KEY

# Backend API URL
VITE_API_URL=http://127.0.0.1:5000
```

**Start the development server:**

```bash
npm run dev
```
