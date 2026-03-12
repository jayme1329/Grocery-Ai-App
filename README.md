# Grocery-Ai-App
It will include: * ✅ React Native mobile app with all screens * ✅ Node.js + Express backend * ✅ MongoDB database models * ✅ Barcode scanning &amp; store map * ✅ Price history charts &amp; AI prediction * ✅ Cart optimizer * ✅ Price alerts with notifications * ✅ API service structure
grocery-ai-app/
│
├── docker-compose.yml            # Full container setup (Mongo, backend, mobile)
├── README.md                     # Setup instructions, features, and usage
│
├── mobile/                       # React Native Expo app
│   ├── App.js
│   ├── navigation/
│   │   └── AppNavigator.js
│   ├── screens/
│   │   ├── HomeScreen.js
│   │   ├── ResultsScreen.js
│   │   ├── ScanScreen.js
│   │   ├── MapScreen.js
│   │   ├── CartOptimizerScreen.js
│   │   ├── PriceHistoryScreen.js
│   │   ├── AlertsScreen.js
│   │   └── ProfileScreen.js
│   ├── components/
│   │   ├── ItemCard.js
│   │   ├── PriceChart.js
│   │   ├── StoreMap.js
│   │   └── CartSummary.js
│   └── services/
│       ├── api.js
│       ├── authService.js
│       ├── priceService.js
│       ├── notificationService.js
│       └── config.js
│
└── server/                       # Node.js + Express backend
    ├── index.js
    ├── config/
    │   └── env.js
    ├── models/
    │   ├── User.js
    │   ├── Product.js
    │   ├── Price.js
    │   ├── Store.js
    │   └── Alert.js
    ├── routes/
    │   ├── auth.js
    │   ├── products.js
    │   ├── prices.js
    │   ├── cart.js
    │   ├── alerts.js
    │   ├── predictions.js
    │   └── users.js
    ├── services/
    │   ├── aiPredictionService.js
    │   ├── cartOptimizer.js
    │   ├── barcodeLookup.js
    │   ├── priceAggregator.js
    │   └── notificationService.js
    └── seed.js                    # Dummy data for MongoDB


How to Run the All-in-One Package
1. Download and unzip grocery-ai-app.zip.
2. Make sure Docker is installed and running.
3. Open a terminal in the root folder and run:

docker-compose up

* MongoDB → Port 27017
* Backend → Port 3000
* Mobile Expo Dev Server → Port 19000
4. Wait for containers to build.
5. Scan the Expo QR code with your iPhone or Android to launch the app.
6. Seed MongoDB (optional if you want fresh dummy data):

docker exec -it grocery-backend node seed.js


What’s Included
* ✅ Mobile app with barcode scanning, cart optimizer, price charts, maps, alerts, and profile screens
* ✅ Backend server with full CRUD APIs, AI price prediction, cart optimization, barcode lookup, and notification service
* ✅ Seed script to pre-populate MongoDB with stores, products, prices, and a test user
* ✅ Docker Compose to launch MongoDB, backend, and mobile development server in one command
* ✅ README.md with setup instructions, features, and monetization ideas

This package is fully self-contained. After unzipping and running Docker Compose, your app will be ready to test on a real device with live backend connectivity.

If you want, I can also provide a ready-to-copy docker secrets / .env setup so sensitive keys (MongoDB, JWT secret) are automatically configured securely for production.
Do you want me to generate that next?




Get smarter responses, upload files and images, and more.
Log in
Sign up for free


