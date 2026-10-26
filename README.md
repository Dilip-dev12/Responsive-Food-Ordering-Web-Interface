# FOODORA – Responsive Food Ordering Web Interface

FOODORA is a complete, modern, fully-responsive Food Ordering Web Application built with React.js, Vite, and Tailwind CSS. Designed with a commercial real-world food delivery visual identity, it features comprehensive state management via Context API and LocalStorage persistence.

---

## 🌟 Key Features

- 🍔 **Complete Food Catalog**: 30+ food items spanning Burgers, Pizza, Indian, South Indian, Chinese, Biryani, Snacks, Desserts, and Beverages.
- 🏪 **Partner Restaurants**: Detailed restaurant profiles, ratings, delivery times, price ranges, and menu filtering.
- 🔍 **Real-Time Search & Filtering**: Multi-criteria filtering by category, veg/non-veg preference, price range slider, star rating, and sort order (popular, rating, price low to high, price high to low).
- 🛒 **Functional Shopping Cart**: Interactive quantity controls, item removals, live subtotal, GST (5%) calculation, delivery fees, and grand total.
- 🎟️ **Working Coupon System**: Real JavaScript discount application (`FOOD10` for 10% off, `WELCOME50` for ₹50 off, `FREEDEL` for Free Delivery).
- 💳 **Checkout & Order Flow**: Full delivery address form validation, payment method selector (COD, UPI, Card), and order placement.
- 📍 **Live Order Tracker**: Interactive visual status timeline (Order Placed ➔ Confirmed ➔ Preparing ➔ Out for Delivery ➔ Delivered) with a live demo status advance button.
- 📜 **Order History**: Persistent order logs saved to LocalStorage with instant Reorder functionality.
- ❤️ **Favorites & Wishlist**: Bookmark favorite dishes with single-click persistence.
- 🌓 **Dark & Light Mode**: Seamless theme toggles saved across browser sessions.
- 📱 **100% Fully Responsive**: Pixel-perfect layout adaptation for Mobile (360px+), Tablet, and Desktop screens.

---

## 🛠️ Technology Stack

- **Frontend Framework**: React.js 18
- **Build Tool**: Vite
- **Styling**: Tailwind CSS v4
- **Icons**: Lucide React
- **Routing**: React Router DOM (v6)
- **State Persistence**: LocalStorage API
- **Data**: Static JSON Datasets (`foods.js`, `restaurants.js`, `offers.js`)

---

## 📁 Project Architecture

```
src/
├── components/          # Reusable UI components
│   ├── Button.jsx       # Flexible button component
│   ├── CartItem.jsx     # Cart item component
│   ├── CategoryCard.jsx # Category pill component
│   ├── EmptyState.jsx   # Generic empty state graphic
│   ├── FoodCard.jsx     # Food item card with actions
│   ├── Footer.jsx       # Global footer
│   ├── LoadingSpinner.jsx # Skeleton loader
│   ├── Modal.jsx        # Confirmations modal
│   ├── Navbar.jsx       # Responsive header & drawer
│   ├── OfferCard.jsx    # Promo coupon card
│   ├── OrderCard.jsx    # Order history card
│   ├── OrderTracker.jsx # Visual order status stepper
│   ├── QuantitySelector.jsx # Counter buttons
│   ├── Rating.jsx       # Star rating badge
│   ├── RestaurantCard.jsx # Restaurant profile card
│   └── SearchBar.jsx    # Live search input
├── context/             # Global React Contexts
│   ├── CartContext.jsx  # Cart state & discount logic
│   ├── FavoritesContext.jsx # Wishlist persistence
│   ├── OrderContext.jsx # Placed orders manager
│   ├── ThemeContext.jsx # Light / Dark mode toggle
│   └── ToastContext.jsx # Floating toast alerts
├── data/                # Mock Datasets
│   ├── foods.js         # 30 detailed food items
│   ├── offers.js        # Coupon codes & promotions
│   └── restaurants.js   # 8 partner restaurants
├── layouts/
│   └── MainLayout.jsx   # Main route wrapper
├── pages/               # 14 Full Page Views
│   ├── Cart.jsx
│   ├── Checkout.jsx
│   ├── Favorites.jsx
│   ├── FoodDetails.jsx
│   ├── Home.jsx
│   ├── Menu.jsx
│   ├── Offers.jsx
│   ├── OrderSuccess.jsx
│   ├── Orders.jsx
│   ├── Profile.jsx
│   ├── RestaurantDetails.jsx
│   ├── Restaurants.jsx
│   ├── Settings.jsx
│   └── TrackOrder.jsx
├── App.jsx              # Router configuration
├── index.css            # Tailwind directives & animations
└── main.jsx             # React DOM entrypoint
```

---

## 🚀 Installation & Running Locally

### Prerequisites
Make sure you have **Node.js** (v16 or higher) and **npm** installed.

### Step 1: Install Dependencies
```bash
npm install
```

### Step 2: Start Development Server
```bash
npm run dev
```

The application will be available at `http://localhost:5173` (or the URL output by Vite).

---

## 💡 Note
This is a complete frontend mini project demo using **LocalStorage** for data persistence. It requires **no backend server or database** to run smoothly.
