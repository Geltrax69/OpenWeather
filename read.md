# Advanced Frontend Assessment: API & State Management

# Assessment 3: Interactive Weather & Packing Planner

> **Difficulty:** Advanced-Intermediate
> **Duration:** 2.5–3 Hours (Live)
> **Focus:** API Integration • State Management • Responsive Design • Dynamic Theming • Modern UI/UX

---

# Objective

Build a **modern, responsive Weather & Packing Planner** that demonstrates strong frontend engineering skills.

The application should resemble a production-ready weather dashboard rather than a basic coding challenge.

We are evaluating both **engineering quality** and **user experience**.

Candidates are encouraged to create a polished interface with thoughtful layouts, smooth animations, and excellent responsiveness.

---

# Design System

Use **Google Material Design** principles for the overall UI.

### Icons

Use **Google Material Symbols** or **Material Icons** throughout the application instead of emojis.

Recommended icons include:

| Purpose     | Material Icon       |
| ----------- | ------------------- |
| Weather     | `partly_cloudy_day` |
| Search      | `search`            |
| Location    | `location_on`       |
| Wind        | `air`               |
| Humidity    | `water_drop`        |
| Temperature | `device_thermostat` |
| Visibility  | `visibility`        |
| Pressure    | `compress`          |
| Packing     | `backpack`          |
| Forecast    | `calendar_month`    |
| Error       | `error_outline`     |
| Success     | `check_circle`      |
| Loading     | `progress_activity` |
| Settings    | `settings`          |

Use the official Material Symbols font:

```html
<link
rel="stylesheet"
href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined" />
```

Example

```html
<span class="material-symbols-outlined">
search
</span>

<span class="material-symbols-outlined">
partly_cloudy_day
</span>
```

---

# UI Requirements

The application should feel like a polished Material Design dashboard.

Recommended characteristics:

* Material Design cards
* 16–24px border radius
* Soft elevation (box-shadow)
* Consistent 8px spacing system
* Material typography
* Smooth transitions (150–300ms)
* Clean responsive layout
* Professional color palette

Avoid decorative emojis anywhere in the interface.

---

# Header

Include:

* Material weather icon
* Application title
* Optional current date
* Optional theme toggle

Example

```
[partly_cloudy_day]

Weather & Packing Planner

Plan your day before you step outside.
```

---

# Search Section

Required

* Search input
* Search button
* Material Search icon
* Placeholder text

Nice additions

* Search icon inside input
* Enter key support
* Animated focus state
* Previous search suggestions

---

# Current Weather Card

Display:

* City
* Country
* Material weather icon
* Temperature
* Feels Like
* Condition
* Humidity
* Wind Speed

Bonus

* Pressure
* Visibility
* Sunrise/Sunset

Suggested icons

| Data        | Material Icon       |
| ----------- | ------------------- |
| Temperature | `device_thermostat` |
| Humidity    | `water_drop`        |
| Wind        | `air`               |
| Visibility  | `visibility`        |
| Pressure    | `compress`          |

---

# Packing Recommendations

Display recommendations as checklist cards or chips.

Each recommendation should include a Material icon.

Examples

| Recommendation      | Icon         |
| ------------------- | ------------ |
| Umbrella            | `umbrella`   |
| Heavy Coat          | `checkroom`  |
| Gloves              | `front_hand` |
| Waterproof Boots    | `hiking`     |
| Sunscreen           | `wb_sunny`   |
| Breathable Clothing | `styler`     |

The list must completely refresh when searching a new city.

---

# Three-Day Forecast

Each forecast card should include:

* Date
* Material weather icon
* High temperature
* Low temperature
* Condition

Cards should animate smoothly into view.

---

# Dynamic Theme

Use CSS Variables.

Never hardcode theme classes per city.

Suggested mappings:

| Weather      | Theme          |
| ------------ | -------------- |
| Clear        | Orange / Amber |
| Clouds       | Neutral Gray   |
| Rain         | Blue           |
| Snow         | Ice Blue       |
| Thunderstorm | Deep Purple    |
| Mist/Fog     | Slate          |

Smoothly animate theme transitions.

---

# Loading State

Display one of:

* Circular Progress Indicator
* Skeleton Cards
* Linear Progress Bar

Disable the search button while fetching data.

Remove stale content before rendering new results.

---

# Error State

Use a Material error icon together with a friendly message.

Example

```
[error_outline]

City not found.

Please check the spelling and try again.
```

---

# Responsive Design

Desktop

* Two-column dashboard
* Forecast cards in one row

Tablet

* Responsive grid

Mobile

* Single-column layout
* No horizontal scrolling

Test widths:

* 1440px
* 1024px
* 768px
* 375px

---

# UI Polish

Include subtle Material-style interactions:

* Hover elevation
* Ripple effect (optional)
* Card transitions
* Button animations
* Skeleton loading
* Fade-in content
* Smooth theme transitions

Avoid excessive animations.

---

# Accessibility

The application should follow basic accessibility practices.

Include:

* Proper labels
* Keyboard navigation
* Visible focus states
* Semantic HTML
* Sufficient color contrast
* Alt text where applicable

---

# What We're Looking For

A strong submission should resemble a small production application.

We value:

* Clean architecture
* Material Design consistency
* Responsive layouts
* Excellent UX
* Maintainable code
* Proper state management
* Accessibility
* Attention to detail
