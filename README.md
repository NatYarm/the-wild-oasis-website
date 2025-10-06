# 🏨 The Wild Oasis - Guest Website

A modern, customer-facing hotel booking website built with Next.js, allowing guests to explore luxury cabins, make reservations, and manage their bookings.

## 🌟 Features

- **Cabin Catalog** - Browse all available luxury cabins with detailed information
- **Cabin Details** - View high-quality photos, amenities, pricing, and availability
- **Guest Reservations** - Book cabins for specific dates with real-time availability
- **User Authentication** - Secure Google OAuth login for guests
- **Guest Area** - Personal dashboard to view and manage bookings
- **Profile Management** - Update personal information and preferences
- **Responsive Design** - Seamless experience across all devices
- **Server-Side Rendering** - Fast page loads and SEO optimization
- **Dynamic Routing** - Clean URLs for each cabin and booking

## 🚀 Demo

**Live Demo:** [View Website](https://the-wild-oasis-website-ten-zeta.vercel.app/)

### Test the Application

1. Click "Login with Google" to authenticate
2. Browse available cabins
3. Select dates and make a reservation
4. View your bookings in the guest area

## 🛠️ Built With

- **Next.js 14** - React framework with App Router
- **React** - UI library
- **Supabase** - Backend, database, and authentication
- **Google OAuth** - Secure authentication provider
- **Tailwind CSS** - Utility-first CSS framework
- **date-fns** - Date manipulation and formatting
- **Hero Icons** - Beautiful SVG icons
- **Vercel** - Deployment platform

## 📦 Installation

1. **Clone the repository**

```bash
git clone https://github.com/NatYarm/the-wild-oasis-website.git
cd the-wild-oasis-website
```

2. **Install dependencies**

```bash
npm install
```

3. **Set up environment variables**

Create a `.env.local` file in the root directory:

```env
# Supabase
SUPABASE_URL=your_supabase_url
SUPABASE_KEY=your_supabase_anon_key

# Google OAuth
AUTH_GOOGLE_ID=your_google_client_id
AUTH_GOOGLE_SECRET=your_google_client_secret

# NextAuth
NEXTAUTH_URL=http://localhost:3000
NEXTAUTH_SECRET=your_nextauth_secret
```

4. **Set up Supabase**

- Create a Supabase project
- Set up the database schema (tables for cabins, bookings, guests)
- Configure Google OAuth in Supabase Authentication settings

5. **Run the development server**

```bash
npm run dev
```

6. **Open your browser**
   Navigate to `http://localhost:3000`

## 🏗️ Build for Production

```bash
npm run build
npm start
```

## 📱 Usage

### For Guests

**Browsing Cabins**

- View all available cabins on the home page
- Filter by capacity or price range
- Click on any cabin to see detailed information

**Making Reservations**

1. Sign in with your Google account
2. Select a cabin
3. Choose your check-in and check-out dates
4. Review the price breakdown
5. Add number of guests and any observations
6. Confirm your reservation

**Managing Bookings**

- Access your guest area from the navigation
- View all upcoming and past reservations
- Edit reservation details (dates, guests, observations)
- Delete reservations if needed

**Profile Settings**

- Update your nationality
- Add or modify your National ID
- These details are used for all future bookings

## 🎨 Key Features in Detail

### Server Components

- Leverages Next.js App Router for optimal performance
- Server-side data fetching for faster initial page loads
- Automatic code splitting and optimization

### Authentication

- Secure Google OAuth integration
- Session management with NextAuth
- Protected routes for guest area

### Booking System

- Real-time availability checking
- Date range selection with validation
- Dynamic pricing based on cabin and duration
- Breakfast options and special requests

### Responsive Design

- Optimized images with Next.js Image component
- Smooth animations and transitions

## 📂 Project Structure

```
the-wild-oasis-website/
├── app/
│   ├── _components/    # Shared components
│   ├── _lib/          # Utility functions and data services
│   ├── about/         # About page
│   ├── account/       # Guest area (protected)
│   ├── cabins/        # Cabin listing and details
│   ├── api/           # API routes
│   ├── layout.js      # Root layout
│   └── page.js        # Home page
├── public/            # Static assets (images, icons)
├── styles/            # Global styles
└── package.json
```

## 🔐 Environment Variables

| Variable             | Description                            |
| -------------------- | -------------------------------------- |
| `SUPABASE_URL`       | Your Supabase project URL              |
| `SUPABASE_KEY`       | Supabase anonymous key                 |
| `AUTH_GOOGLE_ID`     | Google OAuth client ID                 |
| `AUTH_GOOGLE_SECRET` | Google OAuth client secret             |
| `NEXTAUTH_URL`       | Your app URL (production or localhost) |
| `NEXTAUTH_SECRET`    | Secret for JWT encryption              |

## 🚀 Deployment

### Deploy to Vercel (Recommended)

1. Push your code to GitHub
2. Import the project in Vercel
3. Add environment variables in Vercel project settings
4. Deploy!

```bash
# Or use Vercel CLI
npm i -g vercel
vercel
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author

**Natalia Tjoonk | Yarmolinskaya**

- GitHub: [@NatYarm](https://github.com/NatYarm)

## 🔗 Related Projects

- [The Wild Oasis Admin Dashboard](https://github.com/NatYarm/the-wild-oasis-js) - Staff management application

## 🙏 Acknowledgments

- Project inspired by Jonas Schmedtmann's Next.js course

---
