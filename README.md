# OOPs Flashcards

An interactive web-based flashcard application specifically designed for learning Object-Oriented Programming concepts. This application provides a clean, responsive interface with smooth animations and multiple ways to interact with the flashcards.

## Features

### Core Functionality
- **Interactive Flashcards**: Click to flip between term and definition
- **Navigation Controls**: Move between cards using buttons or keyboard shortcuts
- **Shuffle Feature**: Randomize the order of flashcards for better learning
- **Progress Tracking**: Shows current card position in the deck
- **Responsive Design**: Works seamlessly across different devices and screen sizes

### User Interface
- **Clean Dark Theme**: Easy on the eyes with a modern dark color scheme
- **Smooth Animations**: Polished card flip and shuffle animations
- **Centered Layout**: Optimal viewing experience with centered content
- **Touch-Friendly**: Minimum touch target sizes for better mobile experience

### Interactive Controls
1. **Card Navigation**
   - Next/Previous buttons
   - Left/Right arrow keys
   - Touch gestures

2. **Card Flipping**
   - Click/Tap on card
   - Space bar or Enter key

3. **Shuffle Function**
   - Dedicated shuffle button
   - 'S' key shortcut

## Technical Implementation

### CSS Features
- CSS Grid layout system
- Flexbox for component alignment
- CSS Variables for consistent styling
- Responsive units (clamp, vmin, dvh)
- Hardware-accelerated animations
- Media queries for different screen sizes

### JavaScript Architecture
- Object-Oriented design using ES6 class
- Event delegation pattern
- Async/await for data loading
- Fisher-Yates shuffle algorithm
- Debounced animations

### Responsive Breakpoints
- Desktop (>= 768px)
- Landscape mode optimization
- Small screen adaptations
- High DPI screen support

## Data Structure

The application expects a `flashcards.json` file with the following structure:

```json
[
  {
    "term": "String",
    "description": "Definition of the term"
  }
]
```

## Keyboard Shortcuts

| Key           | Action                |
|---------------|----------------------|
| Left Arrow    | Previous card        |
| Right Arrow   | Next card            |
| Space/Enter   | Flip card            |
| S             | Shuffle deck         |

## Browser Support

- Modern browsers with CSS Grid support
- Hardware acceleration for animations
- Touch event support for mobile devices

## Performance Optimizations

1. **Animation Performance**
   - Using transform for animations
   - Hardware acceleration via `transform-style: preserve-3d`
   - Optimized box-shadows for high DPI screens

2. **Responsive Design**
   - Dynamic text sizing using clamp()
   - Optimized layouts for different orientations
   - Efficient media queries

3. **Event Handling**
   - Debounced shuffle animation
   - State management for preventing animation conflicts

## Setup Instructions

1. Clone the repository
2. Create a `flashcards.json` file in the root directory
3. Add your flashcard content following the data structure above
4. Serve the files using a web server
5. Open `index.html` in a modern browser

## Customization

The application uses CSS variables for easy customization:

```css
:root {
    --spacing-xs: 0.25rem;
    --spacing-sm: 0.5rem;
    --spacing-md: 1rem;
    --spacing-lg: 1.5rem;
    --spacing-xl: 2rem;
    --card-border-radius: 12px;
    --container-padding: max(1.7rem, 4vw);
}
```

Modify these variables to adjust spacing, sizing, and overall layout of the application.

## Best Practices Implemented

- Semantic HTML structure
- Accessible button sizes
- Keyboard navigation support
- Responsive design principles
- Performance-optimized animations
- State management for user interactions
- Error handling for data loading
- Cross-browser compatibility considerations

## License

This project is open source and available under the MIT License.
