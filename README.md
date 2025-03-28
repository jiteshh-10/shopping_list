# Shopping List App

<img src="screenshots/app_icon.png" alt="Shopping List App Icon" width="100"/>

## Overview
The Shopping List App is a comprehensive grocery management solution that allows users to create, organize, and manage shopping lists by categories. With real-time data synchronization and an intuitive interface, this app streamlines the shopping experience and helps users stay organized.

## Features

### List Management
- **Category-based Organization**: Separate items by categories (vegetables, fruits, meat, dairy, carbs, sweets, spices, convenience, hygiene, other)
- **Quick Add**: Rapidly add items to appropriate categories
- **Edit & Delete**: Modify or remove items as needed
- **Quantity Control**: Specify amounts and units for each item
- **Priority Marking**: Highlight essential items
- **Check-off System**: Mark items as purchased during shopping

### Data Synchronization
- **Real-time Updates**: Changes sync immediately to backend
- **HTTP Integration**: RESTful API communication for data persistence
- **Offline Support**: Continue using the app without internet connection
- **Data Backup**: Protection against data loss

### User Experience
- **Intuitive Interface**: Clean, user-friendly design
- **Sort Options**: Arrange items by name, category, or priority
- **Search Functionality**: Quickly find specific items
- **Shopping Mode**: Optimized view for use while shopping
- **Multi-list Support**: Create and manage multiple shopping lists

### Additional Features
- **List Sharing**: Share lists with family members or roommates
- **Recipe Integration**: Add all ingredients from a recipe with one tap
- **Recurring Items**: Set frequently purchased items to automatically reappear
- **Budget Tracking**: Optional price fields for expense monitoring
- **Dark/Light Themes**: Customizable visual experience

## Technologies Used
- **Flutter & Dart**: Cross-platform framework for the frontend
- **HTTP Package**: API communication for data operations
- **Provider Pattern**: State management across the application
- **Custom Widgets**: Specialized UI components for shopping functionality
- **Firebase (optional)**: Backend services for data storage

## Screenshots

<div style="display: flex; flex-wrap: wrap; gap: 10px;">
    <img src="screenshots/home_screen.png" alt="Home Screen" width="200"/>
    <img src="screenshots/category_view.png" alt="Category View" width="200"/>
    <img src="screenshots/add_item.png" alt="Add Item" width="200"/>
    <img src="screenshots/shopping_mode.png" alt="Shopping Mode" width="200"/>
    <img src="screenshots/multi_list.png" alt="Multiple Lists" width="200"/>
</div>

## Project Structure
```
lib/
├── models/
│   ├── grocery_item.dart
│   ├── category.dart
│   └── shopping_list.dart
├── providers/
│   └── shopping_list_provider.dart
├── screens/
│   ├── lists_overview_screen.dart
│   ├── list_detail_screen.dart
│   ├── shopping_mode_screen.dart
│   └── new_item_screen.dart
├── services/
│   └── shopping_list_service.dart
└── widgets/
    ├── category_grid.dart
    ├── grocery_item_tile.dart
    ├── new_item_form.dart
    └── category_filter.dart
```

## Installation

1. Clone this repository
```bash
git clone https://github.com/jiteshh-10/shopping_list.git
```

2. Navigate to the project directory
```bash
cd shopping_list
```

3. Install dependencies
```bash
flutter pub get
```

4. Run the app
```bash
flutter run
```

## API Integration
The app uses HTTP requests to communicate with a backend service for data persistence. The following API endpoints are utilized:

- `GET /shopping-lists`: Fetch all shopping lists
- `POST /shopping-lists`: Create a new shopping list
- `GET /shopping-lists/{id}`: Fetch a specific shopping list
- `PUT /shopping-lists/{id}`: Update a shopping list
- `DELETE /shopping-lists/{id}`: Delete a shopping list
- `POST /shopping-lists/{id}/items`: Add an item to a shopping list

## Future Enhancements
- Voice input for adding items
- Image recognition for adding items from photos
- Smart suggestions based on previous shopping patterns
- Geolocation features for store-specific lists
- Nutrition information for food items

## Contribution
Contributions, issues, and feature requests are welcome. Feel free to check the [issues page](https://github.com/jiteshh-10/shopping_list/issues) if you want to contribute.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
