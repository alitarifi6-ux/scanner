# To-Do List Application

A modern, fully-functional to-do list application with local storage persistence. Built with vanilla HTML, CSS, and JavaScript.

## Features

✨ **Core Functionality**
- ✅ Add, complete, and delete tasks
- 💾 **Local Storage Persistence** - Tasks are saved automatically and persist across browser sessions
- 🔍 **Filter Options** - View All, Active, or Completed tasks
- 📊 **Statistics** - Track total and completed tasks
- 🗑️ **Bulk Actions** - Clear completed tasks or all tasks at once

🎨 **User Experience**
- Beautiful gradient UI with modern design
- Smooth animations and transitions
- Fully responsive (mobile-friendly)
- Task creation timestamps
- Empty state messaging
- Keyboard support (Enter to add task)
- XSS protection with HTML escaping

🚀 **Technical Features**
- Pure vanilla JavaScript (no dependencies)
- Object-oriented architecture with TodoApp class
- Error handling for localStorage operations
- ARIA labels for accessibility

## How to Use

1. **Add a Task**
   - Type your task in the input field
   - Click "Add Task" or press Enter

2. **Complete a Task**
   - Click the checkbox next to a task to mark it as complete
   - Completed tasks will have a strikethrough style

3. **Delete a Task**
   - Click the "Delete" button next to any task

4. **Filter Tasks**
   - Use the filter buttons to view:
     - **All**: All tasks
     - **Active**: Only incomplete tasks
     - **Completed**: Only completed tasks

5. **Manage Tasks**
   - **Clear Completed**: Removes all completed tasks
   - **Clear All**: Removes all tasks (with confirmation)

## Local Storage

Your tasks are automatically saved to your browser's local storage:
- Data is stored under the key: `todos_app_data`
- Persists across browser sessions and tab refreshes
- No server or database required

## Browser Compatibility

- Chrome/Edge: ✅
- Firefox: ✅
- Safari: ✅
- Opera: ✅
- Mobile browsers: ✅

## File Structure

```
todo-app/
├── index.html      # HTML structure
├── style.css       # Styling and responsive design
├── script.js       # Application logic
└── README.md       # This file
```

## Responsive Design

The application is fully responsive and works seamlessly on:
- Desktop screens (1024px+)
- Tablets (768px - 1023px)
- Mobile phones (below 768px)

## Storage Limits

Local storage typically allows 5-10MB per domain. For a to-do list application, this translates to thousands of tasks before reaching the limit.

## Privacy

All data is stored locally in your browser. No data is sent to any server or external service.

## Development Notes

The application uses a class-based structure (`TodoApp`) that handles:
- DOM manipulation
- Event listeners
- Local storage operations
- Data filtering and rendering

### Key Methods
- `addTodo()` - Add a new task
- `deleteTodo(id)` - Remove a task
- `toggleTodo(id)` - Mark as complete/incomplete
- `setFilter(filter)` - Change active filter
- `render()` - Update the DOM
- `saveToStorage()` - Persist data
- `loadFromStorage()` - Retrieve saved data

## Future Enhancements

Possible improvements:
- Task priority levels
- Due dates with reminders
- Task categories or tags
- Dark mode toggle
- Export/import functionality
- Cloud sync across devices

## License

Free to use and modify.
