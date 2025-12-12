# Dataset Documentation

This document provides a comprehensive description of all datasets included in the repository.  
All datasets are synthetic but modeled on **foods commonly consumed in Saudi Arabia**, along with relevant nutritional and health-related fields.

---

## 1. Purpose of the Datasets

The datasets in this repository are designed to support research in:

- **Nutritional analytics**  
- **Diet recommendation systems**  
- **AI/ML models for food classification and calorie prediction**  
- **Public health studies related to common Saudi dietary patterns**  
- **Data preprocessing, visualization, and model benchmarking**

All datasets approximate realistic values but do **not** contain real personal information, ensuring they are fully safe for academic and open-source use.

---

## 2. Dataset Overview

### 2.1 `food_items_sa.csv`

A synthetic dataset listing common food items eaten in Saudi Arabia.

| Attribute | Description |
|----------|-------------|
| `food_id` | Unique identifier (integer) |
| `name` | Name of the food item |
| `category` | Food category (Rice, Meat, Bread, Dessert, etc.) |
| `cuisine_origin` | Saudi, Yemeni, Levantine, Indian, etc. |
| `typical_consumption` | Typical serving size eaten (grams) |
| `calories_per_100g` | Calorie value per 100g |
| `is_traditional` | Indicates if the dish is traditionally Saudi (yes/no) |

- **Rows**: 20  
- **Columns**: 7  
- **Source**: Fully synthetic; values modeled on public nutrition tables.

---

### 2.2 `nutrition_values_sa.csv`

Provides nutritional breakdown for foods listed in `food_items_sa.csv`.

| Attribute | Description |
|----------|-------------|
| `food_id` | Foreign key referencing the food item |
| `protein_g` | Protein per 100g |
| `carbs_g` | Carbohydrates per 100g |
| `fat_g` | Fat per 100g |
| `fiber_g` | Fiber per 100g |
| `sodium_mg` | Sodium content |
| `sugar_g` | Sugar content |

- **Rows**: 20  
- **Columns**: 7  
- **Source**: Synthetic; ranges based on standard GCC nutrition sources.

---

### 2.3 `meal_patterns_sa.csv`

Represents common meal combinations in Saudi Arabia.

| Attribute | Description |
|----------|-------------|
| `meal_id` | Unique identifier |
| `meal_name` | Breakfast, Lunch, Dinner, Snack |
| `main_food_id` | Primary food item ID |
| `side_food_id` | Secondary or side dish item |
| `avg_consumption_g` | Average total grams consumed |
| `occasion` | Daily meal, weekend, Ramadan, etc. |

- **Rows**: 12  
- **Columns**: 6  
- **Source**: Synthetic; based on typical Saudi dietary habits.

---

### 2.4 `user_health_profiles.csv` (Optional Synthetic Dataset)

Useful for training recommendation models.

| Attribute | Description |
|----------|-------------|
| `user_id` | Unique synthetic user ID |
| `age` | Age in years |
| `gender` | Male/Female |
| `height_cm` | Height |
| `weight_kg` | Weight |
| `activity_level` | Sedentary, Moderate, Active |
| `preferred_food_category` | Rice, Meat, Bread, Dessert, etc. |

- **Rows**: 25  
- **Columns**: 7  
- **Source**: Fully synthetic; no real personal data.

---

## 3. Data Source Description

All datasets are:

- **Fully synthetic**
- Modeled on public nutritional references from GCC food consumption patterns
- Free of personal or sensitive information
- Created specifically for **research**, **AI model development**, and **academic use**

No web scraping or real-person data is included.

---

## 4. License

All datasets in this repository are released under:

**Creative Commons Attribution 4.0 International (CC BY 4.0)**

You are free to:

- Share
- Adapt
- Build upon

As long as appropriate credit is given.

---

## 5. Citation

If you use these datasets in your research, please cite the repository:

