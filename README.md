# 🍽️ Meals App

A modern, responsive Flutter application designed to simplify meal planning and recipe discovery. Browse curated dishes across diverse categories, filter by dietary requirements, and curate your personal collection of favorite recipes with seamless navigation and state-driven UI updates.

---

## 🌟 Key Features

| Feature | Description |
| :--- | :--- |
| **Category Browsing** | Grid-based discovery of meals grouped into intuitive categories (Italian, Quick & Easy, Exotic, etc.). |
| **Detailed Recipe View** | Step-by-step preparation steps alongside an itemized list of required ingredients. |
| **Dietary Filters** | Real-time filtering toggles for Gluten-Free, Lactose-Free, Vegetarian, and Vegan preferences. |
| **Favorites Management** | One-tap bookmarking to quickly save and manage preferred meals across sessions. |
| **Fluid Navigation** | Material drawer integration and stack-based transitions between categories, meal listings, and details. |

---

## 🛠️ Architecture & Core Concepts

- **Declarative UI**: Built with responsive Flutter widgets ensuring smooth layout adaptation across different screen sizes.
- **State Management**: Reactive UI updates handling dietary filter adjustments and dynamic favorite toggles.
- **Robust Routing**: Stack-based screen navigation using typed parameters and drawer-based root navigation.
- **Object-Oriented Data Modeling**: Structured Dart models for `Meal` and `Category` entities ensuring type safety and clean separation of concerns.

---

## 📂 Project Structure

```text
meals_app/
├── android/                   # Native Android configuration
├── ios/                       # Native iOS configuration
├── assets/                    # Static assets (images, icons)
├── lib/
│   ├── data/
│   │   └── dummy_data.dart    # Mock category & meal data sets
│   ├── models/
│   │   ├── category.dart      # Category model
│   │   └── meal.dart          # Meal data class & enum definitions
│   ├── screens/
│   │   ├── categories.dart    # Root category grid screen
│   │   ├── filters.dart       # Dietary filters configuration screen
│   │   ├── meal_details.dart  # Recipe steps & ingredients screen
│   │   ├── meals.dart         # Category-specific meal listing
│   │   └── tabs.dart          # Bottom navigation / drawer container
│   ├── widgets/
│   │   ├── category_grid_item.dart
│   │   ├── main_drawer.dart
│   │   └── meal_item.dart     # Custom meal summary card
│   └── main.dart              # Application entry point & theme setup
├── pubspec.yaml               # Dependencies & assets configuration
└── README.md
