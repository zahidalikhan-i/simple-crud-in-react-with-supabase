# Supabase CRUD App with React Router V7




## ⚙️ Tech Stack

- **React** – For building the user interface
- **Vite** – For fast development and optimized builds
- **Tailwind CSS** – For rapid, responsive styling with utility classes
- **TypeScript** – For type safety and modern JavaScript features
- **Supabase** – For real-time database, authentication, and storage
- **React Router V7** – For declarative, configuration-based routing

## ⚡️ Features

- **CRUD Operations:**  
  Seamlessly create, read, update, and delete items stored in Supabase.
  

### Installing Dependencies

bash
npm install


### Running the Development Server

bash
npm run dev


Your app will be running at [http://localhost:5173](http://localhost:5173).


### Sample Supabase  Creation


Create a Supabase Project:
Go to Supabase and sign up or log in.
Create a new project in the Supabase dashboard.
Once the project is created, go to Settings > API in the Supabase dashboard to find your:
Supabase URL (e.g., https://your-project-ref.supabase.co)
Public Anon Key (a long string under anon in the API keys section).
Configure Environment Variables:
In your project directory, create a .env file (or update the existing one) and add the Supabase credentials:

VITE_SUPABASE_URL=https://your-project-ref.supabase.co
VITE_SUPABASE_ANON_KEY=your-public-anon-key

open supabase dashboard and click on sql editor and run this query


CREATE TABLE public.items (
  id SERIAL PRIMARY KEY,
  title TEXT NOT NULL,
  description TEXT NOT NULL,
  created_at TIMESTAMPTZ DEFAULT NOW()
);

