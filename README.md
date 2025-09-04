<!-- @format -->

# React Native Todo App

A simple and elegant todo list application built with React Native, Expo, and
styled with TailwindCSS-inspired design.

## Features

### Core Features

- ✅ Add new tasks with title and optional description
- ✅ Mark tasks as complete/incomplete
- ✅ Delete tasks with confirmation
- ✅ View all tasks in a clean list format
- ✅ Data persistence using AsyncStorage
- ✅ Navigation between Task List and Add Task screens

### UI/UX Features

- 📱 Clean, modern interface
- 🎨 Visual distinction between completed and incomplete tasks
- 🔍 Filter tasks (All, Active, Completed)
- 📊 Task counters for each filter
- 🗑️ Swipe-friendly delete with confirmation
- 📅 Display creation dates
- 📝 Support for task descriptions
- 🎯 Empty state handling

## Installation

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd todo-app
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Start the development server**

   ```bash
   npm start
   # or
   expo start
   ```

4. **Run on device/simulator**
   - For iOS: Press `i` or scan QR code with Camera app
   - For Android: Press `a` or scan QR code with Expo Go app
   - For Web: Press `w`

## Project Structure

```
todo-app/
├── App.js                 # Main app component with navigation
│   ├── screens/
│   │   ├── TaskListScreen.js    # Main task list view
│   │   └── AddTaskScreen.js     # Add new task form
│   └── components/
│       └── TaskItem.js          # Individual task component
├── package.json
└── README.md
```

## Technical Details

### Dependencies

- **React Native & Expo**: Core framework
- **@react-navigation**: Screen navigation
- **@react-native-async-storage**: Local data persistence
- **@expo/vector-icons**: Icon library

### Architecture

- **Functional Components**: Using React hooks for state management
- **AsyncStorage**: Local data persistence
- **Stack Navigation**: Simple screen transitions
- **Component Composition**: Modular, reusable components

### Data Model

```javascript
{
  id: string,           // Unique identifier (timestamp)
  title: string,        // Task title (required)
  description: string,  // Optional description
  completed: boolean,   // Completion status
  createdAt: string     // ISO date string
}
```

## Usage

1. **Adding Tasks**: Tap the blue + button to navigate to the add task screen
2. **Completing Tasks**: Tap on a task to toggle its completion status
3. **Deleting Tasks**: Tap the trash icon and confirm deletion
4. **Filtering**: Use the filter buttons (All, Active, Completed) to view
   specific tasks

## Development Notes

- Tasks are stored locally using AsyncStorage
- Data persists between app launches
- Clean, responsive UI following modern design principles
- Proper error handling and loading states
- Input validation and user feedback

## Potential Enhancements

- [ ] Due dates and reminders
- [ ] Task categories/tags
- [ ] Search functionality
- [ ] Dark theme support
- [ ] Task editing
- [ ] Export/import functionality
- [ ] Unit tests
- [ ] Animations and transitions
